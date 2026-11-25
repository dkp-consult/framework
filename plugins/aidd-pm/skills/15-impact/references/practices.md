# Practices

The team's product practices are the `po-practices` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/po-practices.md`. It does not exist at first. This skill reads two of its headings and seeds only `## Impact`.

| Practice | Applies to |
| --- | --- |
| `## Impact`: typical window per kind of signal | the window proposed at arming |
| `## Impact`: signal known to mislead | flagged when proposed as a signal, with the recorded reason |
| `## Impact`: default thresholds | the rule proposed at arming, still confirmed by the user |
| `## Impact`: confidence rule | the report confidence, in place of the starting confidence of `judgment.md` |
| `## Insights`: registry thresholds and segment definitions | the `measured` registry row; read only |

| Situation | Handling |
| --- | --- |
| file or heading absent | apply the defaults |
| practice clashes with a transversal rule or the registry `high` condition | the rule or the condition wins; report the clash |
| lesson approved, file absent | create it from the [practices template](../assets/po-practices.md) with that lesson |
| lesson approved, file present | hand it to a learning capability with the before and after values |
| nothing approved | write nothing |

One measurement never becomes a practice by itself; only a lesson the user approves is kept.
