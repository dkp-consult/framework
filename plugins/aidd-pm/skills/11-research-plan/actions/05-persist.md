# 05 - Persist

Approve, write, and route one research plan.

## Input

The approved gaps, methods, and kits, or an existing plan and a requested change.

## Process

1. Apply [persistence](../references/persistence.md) and follow its result.
2. Apply [lifecycle](../references/lifecycle.md) to every requested transition.
3. Show the plan, and without write authority stop there.
   - A change to gaps or methods: go to step 7.
4. Fill the [plan template](../assets/research-plan.md) with what was approved.
5. Read the plan back and report the path, changed fields as `before -> after`, and the verification result.
6. Offer the next capability per [handoffs](../references/handoffs.md).
7. Read [qualify](02-qualify.md) when gaps or methods change.

## Output

A plan reference, or the reason no write occurred.

## Rules

- A transition the lifecycle does not allow is refused and the status stays unchanged.
