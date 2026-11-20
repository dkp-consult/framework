# 05 - Finalize

Let the user refine, extend, keep, or persist the Product Brief.

## Input

The draft, its sources, and authority.

## Process

1. Use caller-provided bounded authority or invite revision, discovery, session approval, or persistence.
   - Unauthorized draft: leave the workspace unchanged and end with one open feedback question.
   - Without persistence authority: ask session or persist and wait.
2. Apply [persistence](../references/persistence.md) to resolve authorized files.
3. Require authority for both files in a replacement.
4. Persist authorized files and preserve user edits.
5. Read back every changed brief and report the result.
   - After writing: its stable identity, changed fields as `before -> after`, affected relations, and verification result.
   - Without a write: state that no persisted change occurred.
6. Apply [handoffs](../references/handoffs.md) to the next move.
7. Read [discover](02-discover.md) to learn more, [visualize](03-visualize.md) to change the visual, or [shape](04-shape.md) to revise the brief.

## Output

An authorized Product Brief in session or at its resolved path.

## Rules

- In a replacement, the old brief only becomes `superseded`.
- A written brief sits at the standard path and is usable as an Epic goal or PRD source.
