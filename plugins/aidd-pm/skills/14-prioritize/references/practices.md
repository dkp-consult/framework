# Practices

The team's product practices are the `po-practices` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/po-practices.md`. It starts absent. This skill owns its `## Prioritization` section, which holds the team's ranking method.

| Situation | Handling |
| --- | --- |
| file absent | no method; offer one before any score |
| `## Prioritization` absent | no method; offer one before any score |
| method recorded | apply it as written |
| method approved, file absent | create the file from the [practices template](../assets/po-practices.md) with only `## Prioritization` |
| method approved, file present | write only the `## Prioritization` section; keep every other line |
| recorded method contradicts a transversal rule | keep the rule, report the conflict |
| adaptation other than the method the user wants to keep | hand it to a learning capability with its before and after values |
| another section disagrees with this run | read it, never write it |

Other practice adaptations go through a learning capability; the method is the exception. A method is an explicit user decision, not a learned adaptation, so this skill writes it directly once approved. It is never inferred from past rankings.

An ordering capability that follows project memory can apply the recorded method. Sibling Stories keep the relative order their User Story owner sets.
