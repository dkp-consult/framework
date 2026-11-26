# Delta run

A weekly preparation is incremental: it starts from the latest priorities snapshot of the same product.

| Situation | Handling |
| --- | --- |
| no snapshot for the product | full run on every item in scope |
| latest snapshot made with another method | full run; the method change named |
| item unchanged since the snapshot date | values, evidence, and flags carried, flagged `carried`; no question asked |
| item created after the snapshot date | gathered and scored in full |
| item whose status changed | gathered again |
| item done or cancelled since the snapshot | left out of the ranking; a held order field handled per `change-set.md` |
| insight row, impact report, or research plan new or changed since the date | the criteria it sets gathered again for the items it concerns |
| size or dependency changed | effort or ranking read again for that item |
| unknown recorded in the snapshot now settled | that criterion gathered and scored |
| armed or measuring impact report whose `## Follow-up` section has a release date to confirm or a reading due | the release named among the changes; whether it shipped is asked, and a slipped release moves the related item back for review |

| Detection | Read from |
| --- | --- |
| file artifacts | the git history since the snapshot date |
| tracker items | the tracker's update date |
| recorded unknowns | the snapshot's `## Open unknowns` table |

Questions cover the changes above only. The new snapshot is linked to the latest one per `persistence.md`.
