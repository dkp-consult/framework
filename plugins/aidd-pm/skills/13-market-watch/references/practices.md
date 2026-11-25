# Practices

The team's product practices are the `po-practices` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/po-practices.md`. It starts absent.

| Heading | Read for | Default when absent |
| --- | --- | --- |
| `## Market` | the market standard threshold | the one in `comparison.md` |
| `## Market` | the run cadence | monthly |
| `## Insights` | the registry thresholds, such as what counts as repeated or a segment definition, for every row whatever its origin | the wording in `insights-registry.md` |

| Situation | Handling |
| --- | --- |
| practice recorded under a heading read | it replaces the default |
| practice that would lift the user need cap of `insights-registry.md` | ignored; that cap holds, the conflict is reported |
| practice contradicts a transversal rule | the rule holds, the conflict is reported |
| competitors differ from those journaled at the last run | ask whether the threshold in force still fits |
| threshold or cadence change kept, file absent | create the file from the [practices template](../assets/po-practices.md) with only `## Market` |
| threshold or cadence change kept, file present | hand it to a learning capability with the before and after values |
| change used for this run only | nothing written |

Only a practice the user approves is recorded; one run never sets a practice by itself.
