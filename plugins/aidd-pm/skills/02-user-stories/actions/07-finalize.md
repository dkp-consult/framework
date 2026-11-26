# 07 - Finalize

Approve and persist the Stories, transition them, or keep them in the session.

## Input

The Stories, the change asked of them, and the authority for that change.

## Process

1. Apply [persistence](../references/persistence.md) to select the support and create-or-update route.
2. Apply [lifecycle](../references/lifecycle.md) to every requested state change.
3. Show the draft or change and its status, ask for approval, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: return the proposal and leave the Stories and related artifacts unchanged.
4. Apply [relations](../references/relations.md).
5. Create or update only the authorized Stories and preserve fields outside the authorized change.
6. Read the affected graph back and report the result.
   - Markdown: run `scripts/validate-story.cjs`, next to the loaded `SKILL.md`, on each file written, fix each finding that keeps approved content and validate again, and after 3 passes stop and show what is left.
     - Exit 2: quote the output, then stop.
     - A finding whose fix would drop or change approved content: return it to the user with the diff, and rewrite only on their answer.
   - After a write: each stable identity, changed fields as `before -> after`, affected relations, and the verification result.
   - A draft or no-write result: state that no persisted change occurred.
7. Return every persisted identity, then apply [handoffs](../references/handoffs.md) to the next move.
8. Read [write](03-write.md) when the user asks to revise.

## Output

The session drafts or the created and updated Story identities.

## Rules

- A transition-only request changes state and creates no new draft.
- The parent's reassessment is proposed, never inferred.
- A Markdown write leaves source and parent files unchanged unless separately authorized.
