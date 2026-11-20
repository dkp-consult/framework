# 02 - Finalize

Save the approved PRD.

## Input

One approved PRD draft.

## Process

1. Write to `aidd_docs/tasks/<yyyy_mm>/<yyyy_mm_dd>-<feature_name>-prd.md`, creating the month directory when missing.
2. Read the saved PRD back, confirm the file exists on disk, and report the result.
   - After a write: the PRD identity and the verification result.
   - No write happened: state that no persisted change occurred.

## Output

The saved PRD, or no change if not written.
