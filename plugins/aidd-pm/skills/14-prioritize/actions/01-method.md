# 01 - Method

Resolve what is ranked and settle the method that ranks it.

## Input

A product backlog, a set of its items by path or id, or criteria the user wants to rank with.

## Process

1. Resolve the product backlog and the items to rank, proposing those neither done nor cancelled when the user names none.
   - Every item is a Story under one parent: offer the User Story owner per [handoffs](../references/handoffs.md) and stop with no score and no file written.
   - Items span several products: ask which product to rank and wait, with no score until one is named.
   - Epics mixed with their own children: set the level per [ranking](../references/ranking.md) without asking a question.
   - Criteria only: keep no items and go to step 2.
2. Read `## Prioritization` in the practices file per [practices](../references/practices.md).
   - A method is recorded and the user asks no change: hand it to gather.
3. Offer the usual methods with their proposed mappings from [methods](../references/methods.md), or build one with the user per [custom method](../references/custom-method.md), and wait.
   - Choice refused: stop without a score and leave the practices file unchanged.
4. Confirm that every criterion has a scale, a weight when the formula uses one, an evidence source from [evidence](../references/evidence.md), and a mapping from evidence to points.
   - A criterion lacks one: ask for it and wait.
   - Value/effort without thresholds: ask where high splits from low and wait.
5. Fill the [practices template](../assets/po-practices.md) with the method and write it per `practices.md` once approved.
   - Not authorized: show the method and stop without a score.
   - Criteria only: report the recorded method and stop.
6. Read [gather](02-gather.md).

## Output

The items in scope and one recorded method whose every criterion has a scale, an evidence source, and a mapping.
