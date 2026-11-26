# Rating

## Insight

One sentence: which segment says or does what, in which situation.

| Field | Default |
| --- | --- |
| Frequency | the number of distinct signals behind the insight |
| Segment | every segment its signals come from |
| Repetition threshold | three distinct signals |

## Segments

| Segment | Who |
| --- | --- |
| user | someone using the product |
| buyer | someone deciding or paying for it |
| churned customer | a former customer |
| prospect | someone evaluated, not yet a customer |
| support team | the team answering customers |
| sales team | the team selling to buyers |
| partner | a reseller, integrator, or other third party |

## Confidence

Read top to bottom; the first matching row wins. Without an `observed` signal the result is `low`, whatever the count.

| Confidence | When |
| --- | --- |
| `low` | one source item, fewer signals than the threshold, or no `observed` signal |
| `medium` | the threshold reached within one source category |
| `high` | the threshold reached in total, with signals from at least two source categories |

| Corroboration link | Effect on a `customer` row |
| --- | --- |
| a `measured` row | counts as a second source category, `analytics`, holding observed data |
| a `market` row | never raises it |
