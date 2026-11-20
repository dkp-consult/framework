# 03 - Finalize

Persist or transition the authorized Task.

## Input

One Task, the change asked of it, and the authority for that change.

## Process

1. Apply [persistence](../references/persistence.md) to select the support and identity.
2. Apply [lifecycle](../references/lifecycle.md) to every requested transition.
3. Show the draft or change and its status, ask for approval, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: return the proposal and leave the Task and related artifacts unchanged.
4. Apply [relations](../references/relations.md).
   - The requested `order` value is occupied: return it without choosing another, with no write.
5. Create or update only the authorized Task and preserve unrelated fields.
6. Read the affected graph back and report the result.
   - After a write: the stable identity, changed fields as `before -> after`, affected relations, and the verification result.
   - A draft or no-write result: state that no persisted change occurred.
7. Apply [handoffs](../references/handoffs.md) to the next move.
8. Read [frame](01-frame.md) when the user asks to revise.

## Output

A session draft or one created or updated Task identity.

## Rules

- The reassessment of the parent is proposed, never inferred.
- An approved write sets no unsupported optional field.
- Done requires non-empty done conditions and completion evidence.
