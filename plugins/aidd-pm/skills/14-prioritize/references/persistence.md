# Persistence

A decision snapshot records one prioritization decision. It is written once and never edited.

| Situation | Result |
| --- | --- |
| decision approved, new order | create a snapshot; the change set is handed off |
| decision approved, current order kept | create a snapshot; no change set |
| decision approved, no order field touched | create a snapshot; no change set |
| decision withheld or not authorized | no snapshot |
| a snapshot already exists for the date | create `<yyyy_mm_dd>-2.md`, then the next free number |
| an earlier snapshot ranked the same product | list the latest one under `supersedes`; a short `## Changes since` paragraph names what changed since its date |
| a change in the snapshot is rejected by its owner | the snapshot stays as written; the rejection is reported |
| a later run reverses the decision | a new snapshot, never an edit of this one |

Write a Markdown snapshot as `<yyyy_mm_dd>.md` at its location, the date of the decision. Relation values are project-relative paths or tracker ids.

## Location

Project memory's `backlog.md` says where work items and product artifacts live.

| Situation | Location |
| --- | --- |
| explicit target | use it |
| existing artifact | keep its support and path |
| a row of the `## Representation` table in the `backlog.md` memory file names the artifact | that support and native representation, once confirmed to exist |
| that support holds no file, for a registry or a journal | ask the user; never split one across supports |
| several targets remain | ask the user |
| `backlog.md` absent, or no row names the artifact | the default below; tell the user the default was used |

| Artifact | Default |
| --- | --- |
| priorities snapshot | `aidd_docs/backlog/priorities/` |
| insights registry | `aidd_docs/backlog/insights/` |
| research plan | `aidd_docs/backlog/research/` |
| impact report | `aidd_docs/backlog/impact/` |

Markdown is the only support these skills write today. Naming another one is a project's own integration.
