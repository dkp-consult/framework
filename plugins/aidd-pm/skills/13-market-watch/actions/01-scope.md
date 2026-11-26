# 01 - Scope

Fix what this run watches and what it compares against.

## Input

A request to run the watch, optionally a theme, or competitors the user names.

## Process

1. Check that the material brought is about the market.
   - User feedback instead: offer a synthesis capability per [handoffs](../references/handoffs.md) and stop.
2. Read the `market` rows of the sources registry per [watchlist](../references/watchlist.md).
   - Registry missing or without a `market` row: say so, offer Research plan per `handoffs.md`, or take the competitors the user lists for this run.
   - Research plan chosen: stop on that offer.
   - Neither chosen: report that no watchlist exists and stop.
3. Read each competitor's journal, at its location per [persistence](../references/persistence.md), for its last read dates and previous observations per `watchlist.md`.
   - Competitor journaled but removed from the `market` rows: mark it no longer watched.
4. Set the themes per `watchlist.md`.
5. Settle the market standard threshold in force per [practices](../references/practices.md).
   - `practices.md` asks a question: wait for the answer before scanning.
6. Read [scan](02-scan.md).

## Output

The run scope: each competitor with its sources, access, and last read dates, the competitors no longer watched, the themes, and the threshold in force.

## Rules

- Scope writes nothing.
