# 02 - Review

Challenge whether the Task is distinct and actionable.

## Input

The Task draft and its evidence.

## Process

1. Apply [persistence](../references/persistence.md) to find a match or duplicate.
2. Apply [readiness](../references/readiness.md).
3. Apply [lifecycle](../references/lifecycle.md) without inferring readiness.
4. Apply [relations](../references/relations.md).
5. Invite revision or finalization, or apply [handoffs](../references/handoffs.md).
6. Read [frame](01-frame.md) on a revision, else read [finalize](03-finalize.md).

## Output

A reviewed Task and its next user decision.

## Rules

- Review writes nothing.
- Propose `ready` only when every readiness criterion passes.
- A standalone Task states its reason explicitly and never gets an invented parent.
