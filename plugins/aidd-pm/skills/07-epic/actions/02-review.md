# 02 - Review

Challenge whether the Epic is distinct, coherent, and ready for its next state.

## Input

The Epic draft.

## Process

1. Apply [persistence](../references/persistence.md) to find an existing match, overlap, or contradiction.
2. Apply [readiness](../references/readiness.md) to the complete draft.
3. Test every claim against its source.
   - Outcome or need resting on an assumption with no evidence checkable before building: a finding for [handoffs](../references/handoffs.md).
4. Let the user choose revision, finalization, or a capability from `handoffs.md`.
5. Show a revised Epic or the blocking finding, ending a blocker with one open question.
6. Read [shape](01-shape.md) on a revision, else read [finalize](03-finalize.md).

## Output

A reviewed Epic and its next user decision.

## Rules

- Review writes nothing.
- An outcome or need assumption the user leaves silent is not accepted, and the Epic does not pass readiness.
