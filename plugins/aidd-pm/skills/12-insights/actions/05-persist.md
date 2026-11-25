# 05 - Persist

Approve, write, and route the insights registry of one theme.

## Input

The confronted insights, the theme, the scope, and any adaptation made in this run.

## Process

1. Apply [persistence](../references/persistence.md) to each insight and follow its result.
2. Show the rows to write as the draft, ask for approval, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: stop with the registry unchanged.
   - A regrouping or a rewording: go to step 7.
3. Write what was approved per `persistence.md`.
4. Read the file back and report the result.
   - After a write: the path, each row added or changed as `before -> after`, and the verification result.
5. Offer to keep an adaptation made in this run per [practices](../references/practices.md).
6. Offer the next capability per [handoffs](../references/handoffs.md).
7. Read [cluster](03-cluster.md) when a regrouping or a rewording is asked.

## Output

The registry path, or the reason no write occurred.
