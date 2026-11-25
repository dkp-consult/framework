---
type: impact
status: <armed, measuring, or judged>
source: <Epic or Story path or id>
window_end: <yyyy-mm-dd, or pending>
verdict: <validated, iterate, withdraw, or inconclusive, or omit>
confidence: <high, medium, or low, or omit>
supersedes: <previous report path, or omit>
---

<!-- Fill the placeholders from the run only. Set status per the lifecycle: armed after arming, measuring while the reading is pending, judged once the verdict is approved. At arming, keep Change, Arming, and Follow-up and omit the other sections. Keep Follow-up while the status is armed or measuring, and omit it once judged or cancelled. Omit Deviation and Cancellation when they have nothing to record. Remove this comment. -->

# Impact: <change title>

## Change

<What reaches users, and the release date.>

## Arming

| Signal | Segment | Baseline | Baseline period | Source | Instrumentation | Window | Decision rule |
| --- | --- | --- | --- | --- | --- | --- | --- |
| <signal and expected direction> | <segment> | <value, or none with the reason> | <period, rebuilt from history, or none> | <declared source and access> | <verified, or not instrumented> | <length> | <rule as a checkable sentence> |

Fixed on <yyyy-mm-dd>.

<Only when they apply: early arming with the open decisions to re-check when the Epic reaches ready; a single cut with no iterate zone; a signal not instrumented with the choice made.>

## Follow-up

| Item | Date |
| --- | --- |
| Confirm the release date | <planned release date, or pending> |
| Move the window if the release slips | <new window_end, or none yet> |
| Read the signal | <window_end> |

## Measurement

| Value | Period | Source | Read mode |
| --- | --- | --- | --- |
| <aggregated value> | <window read> | <declared source> | <mcp, cli, export, or manual> |

## Confounders

| Confounder | Found in | Effect |
| --- | --- | --- |
| <confounder, or none found> | <where it was found, or the places checked> | <confidence lowered, verdict made inconclusive, or none> |

## Verdict

<The verdict, the confidence, and the rule as applied to the reading.>

## Deviation

<The user's decision that departs from the verdict or the rule, and the reason given.>

## Cancellation

<Why the measurement is no longer pursued.>
