# 04 - Rank

Order the scored items and find what would flip that order.

## Input

The scored items.

## Process

1. Order the items per [ranking](../references/ranking.md).
2. Apply [sensitivity](../references/sensitivity.md) to the ordered items.
3. List the unknowns whose answer could flip a position.
   - The user chooses to collect first: offer Research plan per [handoffs](../references/handoffs.md) and stop.
4. Fill the capacity the user gives per `ranking.md`, each skipped item with its reason.
   - No capacity given: select nothing.
5. Read [propose](05-propose.md).

## Output

A proposed ranking, each position with its sensitivity, the unknowns that could change it, and the selection when a capacity is given.

## Rules

- Rank writes no file.
