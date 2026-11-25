# 06 - Order

Order the Stories that share a parent, without inventing priority.

## Input

The assessed Stories and available product evidence.

## Process

1. Apply [ordering](../references/ordering.md).
2. Apply [relations](../references/relations.md) to predecessors and blockers.
3. State the evidence behind each proposed position and every tradeoff.
4. Let the user, or the authority the caller provided, change or approve the order.
5. Store only the approved relative order.
6. Read [slice](02-slice.md) when the order calls for a reslice, else read [finalize](07-finalize.md).

## Output

An approved relative order.

## Rules

- With no competition between Stories the action is skipped and adds no order field.
- Each ordered Story has one unique position backed by a source signal or relation.
- An unsupported signal adds no score, priority, or ordering weight.
