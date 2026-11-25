# Signals

A signal is one observation from one source item. An insight rests only on signals.

| Field | Holds |
| --- | --- |
| Observation | what the customer said or did, in one sentence |
| Source link | URL, tracker id, or project-relative path of the item or of the export holding it |
| Date | when it was said or done, else the date of the export holding it |
| Segment | one segment from `rating.md` |
| Category | the registry category of the source |
| Kind | `observed` (a behavior seen in data), `recounted` (a past event told by a customer or a team), or `stated` (an intent, a preference, or an opinion) |

| Item | Handling |
| --- | --- |
| no source link can be given | drop it |
| link or file name embedding a person or customer identifier | cite the source and the item type with a neutral reference, never the identifier |
| no date and no dated export | drop it |
| material pasted without a location | ask where it lives; drop it without one |
| outside the scope period or theme | skip it; it is not counted |
| a team member's own guess, no customer behind it | drop it |
| the same conversation or respondent repeating a point | one signal |
| several distinct points in one item | one signal per point |
