# 02 - Qualify

Keep only the gaps whose answer can change a decision.

## Input

The inventoried assumptions with their coverage.

## Process

1. Apply [qualification](../references/qualification.md) to each `unusable` or `missing` assumption, and discard each gap that gates no decision with its reason.
   - No gap kept: report that nothing needs collecting, write no file, and stop.
2. Order the kept gaps by the weight of the decision each one gates, naming that decision on each.
3. Ask one question when the user's answer could change the kept set or its order, and wait.
4. Read [method](03-method.md).

## Output

The decisive gaps ranked by consequence, and every discarded gap with its reason.
