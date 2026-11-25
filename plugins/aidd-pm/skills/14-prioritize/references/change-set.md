# Change set

One entry per item whose position or priority changes and has an owning field, in the shape a backlog orchestration capability accepts.

| Field | Value here |
| --- | --- |
| identity | the item's stable id, URL, or project-relative path |
| artifact | Epic, Story, Task, Spike, or Defect |
| operation | `order` for a position; `update` for a priority field |
| owner | the capability owning that artifact |
| before | the current position or priority, or absent |
| after | the decided position or priority |
| evidence | the decision snapshot path and the item's score line |

| Situation | Handling |
| --- | --- |
| Epic changing position | `order` entry |
| other item whose owner declares a position across sets | `order` entry |
| other item whose owner declares no such position | no entry; reported as no owning field; its rank stays in the snapshot |
| no decided change touches an order or priority field | no change set; stated, and no hand-off offered; the global rank lives in the snapshot |
| done or cancelled item still holding an order field | entry releasing that field, in the same change set as the decided ranks |
| item living on an external tracker, such as a GitHub board | entry handed only to a backlog orchestration capability, with the product owner's explicit authorization in this run; without it, reported unhandled |
| project support declares a priority field | `update` entry for that field |
| project support declares no priority field | no `update` entry |
| item already at its decided position | no entry |
| current order kept | no change set |
| item whose owner is not installed | entry kept, owner named, reported unhandled |

The change set is handed off, never persisted by this skill.
