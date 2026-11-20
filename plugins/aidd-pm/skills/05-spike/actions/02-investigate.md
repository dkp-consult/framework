# 02 - Investigate

Collect only the evidence that can change the blocked decision.

## Input

A spike eligible for investigation, by id, URL, or path.

## Process

1. Resolve one spike and transition it to `in-progress` when allowed by [lifecycle](../references/lifecycle.md).
   - Terminal Spike: append no attempt.
2. Apply [investigation](../references/investigation.md) with matching [capabilities](../references/capabilities.md).
3. Read [conclude](03-conclude.md).

## Output

Evidence and an outcome status.

## Rules

- A next path the user has not approved keeps the evidence and leaves the status unchanged until the user answers.
- Investigation preserves the attempt history and changes only the Spike.
