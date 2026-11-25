# Insights registry

A judged report feeds the insights registry, `<theme>.md` at its location per `persistence.md`, one living file per theme. This skill adds or updates only rows whose origin is `measured`, and keeps every other section, row, and line as found.

| Column | Value for a measured row |
| --- | --- |
| Insight | the effect in one sentence: the change, the signal, the movement, the window |
| Origin | `measured` |
| Evidence | link to the impact report and the source, with the number of periods or data points read |
| Frequency | how many measurements found this effect |
| Segment | the segment the signal covers, named per the `## Insights` segment definitions when present |
| Confidence | the report confidence, `high` only with a baseline measured at arming and a decision rule fixed at arming |
| Assumption | link to the Epic or User Story, or empty |
| Effect | with a linked assumption, `supports` for `validated` or `iterate` and `contradicts` for `withdraw`; without one, `new` |

| Situation | Handling |
| --- | --- |
| verdict `inconclusive` | no row |
| theme file exists | add or update the measured row there |
| no theme file fits | ask the theme, then create the file from the [insights template](../assets/insights.md) |
| same finding already in a `measured` row | append the evidence, raise the frequency, recompute the confidence; no new row |
| same finding in a `customer` or `market` row | link that row in the Evidence of the measured row |
| new measurement opposite to an earlier one | a new measured row, linking the earlier row in its Evidence |
