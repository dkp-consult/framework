# 02 - Assess

Determine whether the Defect is actionable.

## Input

The Defect draft and available evidence.

## Process

1. Apply [persistence](../references/persistence.md) to detect a match or duplicate.
   - A duplicate: propose the existing identity, with no new Defect.
2. Apply [readiness](../references/readiness.md).
   - A criterion fails: name the missing evidence and keep the Defect `reported`.
3. Apply [lifecycle](../references/lifecycle.md) without inferring confirmation.
4. Apply [relations](../references/relations.md) and invent none.
5. Invite correction or approval of the finding in one open question.
6. Read [capture](01-capture.md) on a revision, else read [finalize](03-finalize.md).

## Output

A readiness finding and proposed lifecycle state.

## Rules

- Assess writes nothing.
- Propose `ready` only when every readiness criterion passes.
