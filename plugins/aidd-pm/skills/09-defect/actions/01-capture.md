# 01 - Capture

Frame one observed mismatch as a Defect report.

## Input

A report, evidence, existing Defect, or current context.

## Process

1. Inspect the supplied source, relevant artifacts, and matching Defects.
   - A matching Defect: return its existing identity, with no duplicate draft.
2. Apply [qualification](../references/qualification.md), and on a mismatch apply [handoffs](../references/handoffs.md), with no draft.
3. Ask one question, with no draft, only when expected behavior, actual behavior, or impact cannot be resolved, choosing a question that can also determine the work type.
4. Fill the [Defect template](../assets/defect-template.md) sections the source supports and leave the rest out, unsupported evidence or reproduction included.
5. Fill the front matter relation keys the context supports per [relations](../references/relations.md), the affected Story under `related_to`, and remove every front matter key with no value.
6. Show the complete report and fold corrections.
7. Read [assess](02-assess.md).

## Output

One Defect draft or one clarification question.

## Rules

- Capture writes nothing.
