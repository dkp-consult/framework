# 02 - Measure

Read the signal once the measurement window has closed.

## Input

An armed or measuring report, a judged or cancelled report with a new measurement asked, or an unarmed change (a released Epic or User Story), by path or id.

## Process

1. Read the report and its frozen elements.
   - Judged or cancelled report: measure its change again as an unarmed change and leave that report unchanged.
   - Unarmed change: resolve its signal per [arming](../references/arming.md).
   - No signal: offer the owning capability per [handoffs](../references/handoffs.md) and stop.
2. Agree, for an unarmed change, the segment, window, and decision rule with the user per `arming.md` before any reading.
3. Compare the end date with today.
   - Window not over: report the end date and stop.
4. Locate the source of the signal per [sources registry](../references/sources-registry.md).
   - No readable source and manual mode refused: stop on the Research plan offer.
   - Export or manual figures still awaited: hand the report to [persist](04-persist.md) as pending, with no verdict.
5. Rebuild, for an unarmed change, the baseline from history per `arming.md`.
   - No history: record that no baseline exists.
6. Read the signal over the whole window.
   - Signal marked `not instrumented`: check that its source now holds its data before it can decide.
   - Deciding signal still unverified at the window end: state the gap and mark the reading not verified.
7. Hand the reading to [judge](03-judge.md).

## Output

The reading over the window, the baseline it is compared with, and the decision rule, each with its origin.

## Rules

- Measure writes no file.
