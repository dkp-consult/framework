# Lifecycle

`status` lives in frontmatter.

| Status | Meaning | May move to |
| --- | --- | --- |
| `armed` | signal, baseline, window, and rule fixed; the window has not been read | `measuring`, `judged`, `cancelled` |
| `measuring` | the window is over and the reading awaits an export or figures | `judged`, `cancelled` |
| `judged` | the verdict, confidence, and confounders are recorded | terminal |
| `cancelled` | the change was dropped or the measurement abandoned, with the reason under `## Cancellation` | terminal |

| Run | First status |
| --- | --- |
| arming | `armed` |
| unarmed change, reading pending | `measuring` |
| unarmed change, reading done | `judged` |

A status moves only when the user asks or confirms it.
