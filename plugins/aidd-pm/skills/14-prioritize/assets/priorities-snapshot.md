---
type: priorities
date: <yyyy-mm-dd>
product: <product or backlog name>
method: <method name>
supersedes: <previous snapshot path, or omit>
---

<!-- Fill every placeholder from the run, one row per item and criterion, omit a section with nothing to say, and remove this comment. -->

# Priorities: <product> on <yyyy-mm-dd>

## Changes since

<What changed since the superseded snapshot: items added, closed, or changed, evidence new or changed, unknowns settled, releases checked.>

## Method

<Method name and formula, as recorded under `## Prioritization` in the practices.>

## Evidence

| Item | Criterion | Value | Evidence | Flag |
| --- | --- | --- | --- | --- |
| <item path or id> | <criterion> | <value, range, or `unknown`> | <links, or none> | <`low`, user assumption, build only, `carried`, or empty> |

## Scores

| Proposed rank | Item | Score | Confidence | Ceiling | Sensitivity |
| --- | --- | --- | --- | --- | --- |
| <n> | <item path or id> | <score or range> | <high, medium, or low> | <lowest Confidence cited> | <what flips it, or stable> |

## Selection

Capacity: <capacity the user gave>

| Item | Selected | Reason |
| --- | --- | --- |
| <item path or id> | <yes or skipped> | <does not fit, dependency, open decision, or empty> |

## Decision

Decided by: <role, or the caller's bounded authority>

| Decided rank | Item | Change |
| --- | --- | --- |
| <n> | <item path or id> | <before -> after, or unchanged> |

## Deviations

| Item | Proposed rank | Decided rank | Reason |
| --- | --- | --- | --- |
| <item path or id> | <n> | <n> | <the reason the user gave> |

## Open unknowns

| Item | Criterion | How it would be settled |
| --- | --- | --- |
| <item path or id> | <criterion> | <research plan link, estimate request, or none yet> |
