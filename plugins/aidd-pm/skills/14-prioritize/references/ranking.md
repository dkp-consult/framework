# Ranking

| Signal | Effect |
| --- | --- |
| higher score | ranks earlier |
| required predecessor | ranks before its dependent whatever the scores, the dependency stated |
| blocked item | ranks after its blocker |
| equal scores | tied; the tie is shown for the user to break |
| overlapping score ranges | undecided between them; the unknown that separates them is named |
| same MoSCoW category | unordered inside it except for dependencies |
| item scored `unclassified` | listed after the classified ones, its unknown named |
| Epics and standalone items | ranked |
| Story or Task whose parent Epic is in scope | not ranked; listed under its parent, so no need counts twice |
| user's scope names an Epic's children to rank | ask which level to rank before any score |

## Capacity

| Situation | Selection |
| --- | --- |
| capacity given, on the effort scale | filled in rank order |
| item larger than the capacity left | skipped as not fitting; the next item considered |
| item whose predecessor is not done or selected before it | skipped, the dependency named |
| item waiting on an open decision | skipped, the decision named |
| item with effort `unknown` | skipped, the missing estimate named |
| no capacity given | no selection |
