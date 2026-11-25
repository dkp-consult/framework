# 01 - Arm

Fix how a change will be judged before it reaches users.

## Input

An Epic moving to `ready`, a User Story about to be released, or an early armed report whose Epic reached `ready`, by path or id.

## Process

1. Read the change and resolve its signal per [arming](../references/arming.md).
   - Nothing identifies the change: ask one question and wait, with nothing frozen.
   - No signal: offer the owning capability per [handoffs](../references/handoffs.md) and stop with no file written.
   - Already released: continue with [measure](02-measure.md) as an unarmed change.
   - Epic not yet `ready` and no early arming asked: say arming waits for `ready` and stop.
   - Early arming asked: list the open decisions that could change the signal and note the early arming.
   - Early armed report whose Epic reached `ready`: re-check its open decisions and propose the arming again.
2. Read the `## Impact` heading of the practices file per [practices](../references/practices.md).
3. Find a source able to read the signal per [sources registry](../references/sources-registry.md).
   - No readable source and manual mode refused: stop on the Research plan offer.
4. Check that each signal's source has received its data, as `arming.md` defines it.
   - Signal not instrumented: mark it `not instrumented` and ask the user to add the check as work or to choose another source.
   - Another source chosen: return to step 3.
5. Read the baseline as `arming.md` defines it.
   - Baseline source with access `export`: request the export from its owner and stop until it arrives.
   - History too incomplete: propose an absolute threshold and note why no baseline was taken.
6. Propose the segment, window, release date, end date, and a decision rule with distinct `validated` and `withdraw` thresholds, the `iterate` gap, and the `inconclusive` conditions per `arming.md`, then wait for the user's confirmation.
   - Proposal rejected: revise it from the user's answer and propose again, with nothing frozen until confirmed.
   - Single cut insisted on: keep it and note the missing `iterate` zone.
7. Hand the frozen elements, segment included, to [persist](04-persist.md).

## Output

The frozen signal, segment, baseline, window, and decision rule, ready for persist.

## Rules

- Arm writes no file.
