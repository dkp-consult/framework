# Scoring

## Criterion value

| Situation | Value |
| --- | --- |
| cited evidence meets a condition of the recorded mapping | that point, with its links |
| cited evidence meets the conditions of several points | the range, with its links |
| cited evidence meets no condition of the mapping | the point the product owner gives, the evidence cited, flagged user assumption |
| the mapping reads a need level | the level the product owner gives per item, flagged user assumption; never read from the insight text, which states no severity |
| the product owner answers off the recorded scale, such as `low` or `medium` | asked again as a point of the scale; never turned into a range |
| the user states a value in the exchange | that value, flagged user assumption |
| value carried from the latest snapshot | that value, its evidence, and its flags, flagged `carried` |
| material the user supplies, not synthesized into an insights registry | read as the user's assumption |
| value rests on a `low` row | that value, flagged `low` |

## Effort

Effort is the total cost of the item: build, review, maintenance, and support.

| Situation | Effort |
| --- | --- |
| scale named, the estimate covers every cost | that estimate, converted per the recorded mapping when the criterion needs one |
| scale named, the estimate covers build only | that estimate, flagged as build only; the missing costs asked of the team |
| criterion needs a conversion and none is recorded | `unknown` |
| scale named, no estimate on the item | `unknown`; the estimate is asked from the capability owning that artifact |
| no scale in project memory | `unknown` |

## Score

| Situation | Score |
| --- | --- |
| every criterion has a value | the method formula applied |
| a criterion is `unknown` | the range the formula gives over that criterion's whole scale |
| a criterion is `unknown` in MoSCoW | `unclassified` |

## Score confidence

| Confidence | When |
| --- | --- |
| high | every criterion valued, every rated evidence cited `high` |
| medium | every criterion valued, the lowest rated evidence cited `medium` |
| low | a criterion `unknown`, a `low` row cited, or a value resting on the product owner's assessment |

| Ceiling | Rule |
| --- | --- |
| cap | an item's confidence never exceeds the lowest Confidence among the evidence it cites |
| product owner's assessment | counts as `low` |
| evidence without a Confidence, such as an estimate or a relation | does not lower the ceiling |
| display | the ceiling shown next to each score's confidence |

The score confidence is separate from a method's own confidence criterion.
