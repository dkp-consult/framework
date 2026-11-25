# Judgment

## Verdicts

| Verdict | When |
| --- | --- |
| `validated` | the reading meets the `validated` threshold of the rule |
| `iterate` | the reading falls between the `withdraw` and `validated` thresholds |
| `withdraw` | the reading reaches the `withdraw` threshold, or, under a single cut, stays short of it |
| `inconclusive` | a condition the rule names as inconclusive, no baseline for a threshold relative to one, an incomplete window, a changed signal definition, a deciding signal still `not instrumented`, or a confounder able to explain the whole movement |

## Starting confidence

| Confidence | When |
| --- | --- |
| `high` | baseline measured at arming, rule fixed at arming, reading from a declared source over the full window |
| `medium` | baseline rebuilt from history, absolute threshold with no baseline, or rule agreed after release |
| `low` | no baseline for a relative threshold, or figures supplied without any declared source |

The starting level is then lowered by the confounders, never below `low`.
