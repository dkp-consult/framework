# Arming

What is fixed before a change is judged, and where each element comes from.

| Element | Fixed as | Taken from |
| --- | --- | --- |
| Signal | one measurable quantity and the direction expected | the Epic's `Success Evidence` or the User Story's stated metric |
| Segment | the population the signal covers, as a segment name | the change's audience, confirmed by the user |
| Baseline | a value, its period, and its source | the latest complete period of the window's length before arming |
| Instrumentation | `verified` once the source shows the signal's data at least once, else `not instrumented` | the source itself: an event received or an export that exists |
| Window | a length in days or weeks | the `## Impact` practice, else the user |
| Release date | the planned or actual date users get the change | the user |
| End date | release date plus window length, stored as `window_end` | computed |
| Decision rule | a `validated` threshold and a different `withdraw` threshold, the gap between them reading as `iterate`, plus the conditions that make the reading `inconclusive` | proposed at arming, confirmed by the user before release |

| Situation | Handling |
| --- | --- |
| Epic or User Story names no success signal or metric | no signal; nothing is armed |
| Epic not yet `ready` | arming waits for its move to `ready` |
| user asks to arm an Epic before `ready` | arm it as early arming; list the open decisions that could change the signal, to re-check when the Epic reaches `ready` |
| signal names no quantity | ask which figure would show it; never pick one |
| several signals in the Success Evidence | one rule per signal; the user names which one decides |
| source has never received the signal's data | the signal is `not instrumented` and cannot decide until verified; the user chooses between adding the check as work and another source |
| baseline source with access `export` | arming waits for the export; it resumes with the figures once they arrive, and no report is written before |
| history too incomplete for a baseline | an absolute threshold that needs no baseline is valid; record why no baseline was taken |
| user insists on a single cut | record it; the report flags the missing `iterate` zone |
| release date unknown at arming | keep `window_end` as `pending`; it is set when the date is given |
| unarmed change, source holds the period before release | rebuild the baseline from that period, marked as rebuilt |
| unarmed change, no such history | no baseline; state it in the reading |

A decision rule reads as a sentence the user can check later, such as `validated if weekly signups rise 10% within 30 days, withdraw if they rise less than 3%, inconclusive if tracking breaks or the window is cut short`.
