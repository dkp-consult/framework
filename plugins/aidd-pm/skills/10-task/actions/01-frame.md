# 01 - Frame

Define one bounded delivery Task.

## Input

A request, parent artifact, existing Task, or current context.

## Process

1. Inspect the source, relevant artifacts, and matching Tasks.
   - No work can be identified: ask one open question about the outcome, with no draft.
   - A matching Task: return its existing identity, with no duplicate draft.
2. Apply [qualification](../references/qualification.md), and on a mismatch apply [handoffs](../references/handoffs.md), with no Task draft.
3. Ask one question at a time while outcome, scope, completion evidence, or ownership remains blocking.
4. Fill the [Task template](../assets/task-template.md) sections the source supports and leave the rest out.
5. Show the complete draft and fold corrections.
6. Read [review](02-review.md).

## Output

One Task draft or one clarification question.

## Rules

- Frame writes nothing.
- Optional metadata stays absent unless it is known and the project supports it.
