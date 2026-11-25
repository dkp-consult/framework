# 04 - Assess

Determine each Story's readiness and blockers.

## Input

The Story drafts.

## Process

1. Apply [readiness](../references/readiness.md) to every Story.
2. Apply [handoffs](../references/handoffs.md) and [relations](../references/relations.md).
3. Return an oversized or non-valuable Story to slicing.
4. Use `ready` only when every readiness criterion passes.
   - Any criterion fails: keep `proposed` and list only readiness blockers.
5. Show changed or `proposed` Stories and ask about the highest gap.
   - Set unchanged and ready: continue without intermediate output, never past the approval finalize waits for.
6. Read [slice](02-slice.md) on a reshape, else read [estimation](05-estimation.md).

## Output

The Story documents with their status, and a Spike for any blocking unknown.

## Rules

- Each failed readiness row maps to one sourced gap.
- An unapproved blocker leaves the Story in place, offers a Spike, and leaves related artifacts unchanged.
- An approved blocker Spike names the Story in its `parents`, with no inverse field mirrored.
- Output carries no assessment summary, empty field, tooling gap, or skipped-route report.
