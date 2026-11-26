# Comparison

| Class | When |
| --- | --- |
| `new` | the fact has no previous observation for that competitor |
| `changed` | a previous observation covers the same item with a different value, such as a price or a limit |
| `removed` | a previous observation is no longer found on a source that was read |
| unchanged | same item, same value; not reported |

A source skipped in this run never yields `removed`.

| Market standard | Rule |
| --- | --- |
| item | a capability, a price model, or a policy announced by several competitors |
| host platform | observed and journaled, never counted, neither in the share nor in the watchlist total |
| default threshold | announced by at least 50% of the competitors in the watchlist, host platforms excluded |
| reached | a finding worded `Market standard: <item>`, with the share of the watchlist |
| no longer met | a new finding worded `No longer a market standard: <item>`, linking the earlier row; that row is never edited into the opposite |

| A finding matters when | Example |
| --- | --- |
| it reaches or loses the market standard threshold | most competitors now announce a free tier |
| it bears on an assumption linked in a theme file | a price an assumption rests on changes |
| the user flags it during the run | a launch the user wants tracked |

Any other observation stays in the journal and raises no insight row.

| Effect | When |
| --- | --- |
| `supports` | the finding confirms the assumption its row links |
| `contradicts` | the finding goes against the assumption its row links; the assumption itself is never edited |
| `new` | the row links no assumption |
