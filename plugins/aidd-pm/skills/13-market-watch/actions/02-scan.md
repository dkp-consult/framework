# 02 - Scan

Read each declared source and record what it shows.

## Input

The run scope from scope.

## Process

1. Choose web or manual mode per [scanning](../references/scanning.md).
   - Manual mode: ask the user to paste or export the material, and wait.
   - Material refused: report the skips and stop.
2. Read each source of the scope since its last read per `scanning.md`.
   - Source not readable per `scanning.md`: skip it and record why.
   - No source could be read: report every skip and stop.
3. Turn each fact read into one observation per `scanning.md`.
   - Observation dropped: count it for the report.
4. Read [compare](03-compare.md).

## Output

The observations per competitor, each with its date and URL, every competitor read with nothing to record, and every source skipped and observation dropped, with the reason.

## Rules

- Scan writes nothing.
