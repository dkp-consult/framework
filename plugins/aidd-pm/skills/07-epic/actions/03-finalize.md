# 03 - Finalize

Approve and persist the Epic, transition it, or keep it in the session.

## Input

One Epic, the change asked of it, and the authority for that change.

## Process

1. Apply [persistence](../references/persistence.md) to select the target and create-or-update route.
2. Apply [lifecycle](../references/lifecycle.md) to every requested transition.
3. Show the draft or change and its status, ask for approval, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: return the proposal and leave the Epic and related artifacts unchanged.
4. Apply [relations](../references/relations.md).
5. Create or update exactly one Epic and preserve fields outside the authorized change.
6. Read the affected graph back and report the result.
   - After a write: the stable identity, changed fields as `before -> after`, affected relations, and the verification result.
   - A draft or no-write result: state that no persisted change occurred.
7. Apply [handoffs](../references/handoffs.md) to the next move.
8. Read [shape](01-shape.md) when the user asks to revise.

## Output

The session draft or one created or updated Epic with its links.

## Rules

- The fate of child items is proposed, never inferred.
- An approved write leaves no optional field empty and holds `Cancellation` only when the status is `cancelled`.
- Done requires success evidence that confirms the outcome, and child closure alone is insufficient.
