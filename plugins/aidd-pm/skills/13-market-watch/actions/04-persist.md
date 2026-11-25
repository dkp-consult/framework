# 04 - Persist

Approve, append the journals, and raise the market insights.

## Input

The classed observations, the read lines, the skipped sources, the competitors no longer watched, and the rated findings from compare.

## Process

1. Apply [persistence](../references/persistence.md) and follow its result.
2. Show the journal entries and the insight rows as the draft, ask for approval, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: stop with no journal or registry file changed.
   - A change to observations or findings: go to step 7.
3. Append each journal entry from the [journal template](../assets/journal.md), then write each market row per [insights registry](../references/insights-registry.md).
   - Nothing new: write the journal lines only and report nothing new.
4. Read every written file back and report the result.
   - After a write: each path, changed rows as `before -> after`, the verification result, and the next due date per [practices](../references/practices.md).
5. Offer to keep an approved threshold or cadence change per `practices.md`.
6. Offer the next capability per [handoffs](../references/handoffs.md).
7. Read [compare](03-compare.md) when observations or findings change.

## Output

The journals and theme files written, or the reason no write occurred.

## Rules

- Written files hold no `<` placeholder left from an asset.
