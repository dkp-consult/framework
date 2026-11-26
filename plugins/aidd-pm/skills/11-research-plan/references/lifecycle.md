# Lifecycle

`status` lives in frontmatter.

| Status | Meaning | May move to |
| --- | --- | --- |
| `open` | planned, collection not started | `collecting` once every gap has its decision rule, `cancelled` |
| `collecting` | at least one collection is running | `done`, `cancelled` |
| `done` | every stop condition is met, the material is ready to synthesize | terminal |
| `cancelled` | no longer pursued, with the reason under `## Cancellation` | terminal |

A status moves only when the user asks or confirms it.
