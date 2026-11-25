# 02 - Gather

Fetch, for each item, the evidence each criterion of the method needs.

## Input

The items in scope and the recorded method.

## Process

1. Look for the latest snapshot of the product, at its location per [persistence](../references/persistence.md), and apply [delta run](../references/delta-run.md).
   - No snapshot, or one made with another method: full run on every item in scope.
   - Snapshot found: carry the unchanged lines and keep only the changes since its date for the next steps.
2. Read each item and its relations.
3. Take, for each criterion, the evidence kinds [evidence](../references/evidence.md) names.
4. Read those artifacts for each item and keep every link found.
   - A criterion needs a source category: read the sources registry, the `sources` file of project memory, to see whether it is readable.
   - Registry missing: say so without creating one, offer Research plan or material the user supplies, read as the user's assumption unless routed to a synthesis capability first, and wait.
   - The user chooses to collect first: offer Research plan per [handoffs](../references/handoffs.md) and stop.
   - Raw signals not yet in an insights registry: offer a synthesis capability per `handoffs.md` and continue without them.
   - Market pressure claimed with no market row: offer a market watch capability per `handoffs.md` and continue.
5. Hand every evidence line, an empty or carried one included, with the changes found, to [score](03-score.md).

## Output

One evidence line per item and criterion: the links found, or none, or the line carried from the latest snapshot.

## Rules

- Gather writes no file.
