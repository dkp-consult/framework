# Evidence

Where each kind of criterion evidence lives and what it can set. Each artifact is read at its location per `persistence.md`.

| Kind | Where | Sets |
| --- | --- | --- |
| customer insight | rows with Origin `customer` in the insights registry, `<theme>.md` | reach from Frequency and Segment, value or impact from Effect |
| measured insight | rows with Origin `measured` in the same registry | value or impact, with what was observed after shipping |
| market insight | rows with Origin `market` in the same registry | pressure or time criticality when it names a market standard |
| row confidence | the Confidence column of every row cited | the confidence criterion where the method has one, and the flags |
| estimate | the item's estimate, on the scale project memory names | effort, job size, or ease |
| research plan | its `<slug>.md` | risk reduction when the item settles one of its gaps |
| impact report | its `<slug>.md` | value or impact of similar shipped work, and its confidence |
| item relations | the item's parent, dependencies, and goal | dependencies, obligations, the outcome it serves |
| declared source | a category readable in the sources registry, the `sources` file of project memory | a count read directly, such as reach from analytics |

| Situation | Handling |
| --- | --- |
| research plan `open` or `collecting` for the criterion | the criterion stays `unknown`, the plan linked as pending |
| research plan `done`, not yet synthesized | the criterion stays `unknown`; a synthesis capability is offered |
| assumption marked contradicted in an insight row | cite the contradiction, not the assumption |
| market row about a user need | cite its Confidence as written in the registry |
| several rows for one criterion | cite each; the strongest corroborated one sets the value |
| source category declared with access `none` | unreadable; the criterion stays `unknown` |

Evidence is linked by file and row, never copied.
