# 04 - Persist

Approve, write, and route one impact report.

## Input

The armed elements, a pending reading, or a judgment; or an existing report with a cancellation or a new release date.

## Process

1. Apply [persistence](../references/persistence.md) and follow its result.
2. Apply [lifecycle](../references/lifecycle.md) to every requested transition.
   - Transition not allowed: refuse it and stop with the status unchanged.
3. Show the report.
   - No write authority: stop there with the draft shown.
4. Fill the [impact report template](../assets/impact-report.md) with what was approved.
5. Propose, for a judged report, its row per [insights registry](../references/insights-registry.md) and write it once approved.
6. Read every written file back and report what changed.
   - After a write: the report path, each changed field as `before -> after`, and what the read-back showed.
7. Offer the next move per [handoffs](../references/handoffs.md).
   - Lesson the user wants to keep, such as a typical window or a misleading signal: handle it per [practices](../references/practices.md).

## Output

A report reference, or the reason no write occurred.
