# Handoffs

Each row is an offer made with what was seen; the run stops after it and never triggers the capability. This skill writes only impact reports, `measured` registry rows, and a first practice.

| Observed | Capability | Return |
| --- | --- | --- |
| Epic with no success signal | Epic | arming resumes once the signal is defined |
| User Story with no stated metric | User Story | arming resumes once the metric is stated |
| no sources registry, or no source for the signal | Research plan | one-way; manual mode stays available |
| `armed` or `measuring` report | a prioritization capability | reads its `## Follow-up` at its next run |
| user asks for a reminder | the host | schedules it from the `## Follow-up` dates |
| verdict judged on an Epic | Epic | its owner records what it showed under `Success Evidence` and decides the Epic's status |
| verdict judged on a User Story | User Story | its owner records the result and decides the Story's status |
| verdict `inconclusive` | Research plan | a targeted qualitative collection; a later measurement may follow |
| lesson approved while practices exist | a learning capability | one-way, with the before and after values |
| no match | none | report what was observed |
