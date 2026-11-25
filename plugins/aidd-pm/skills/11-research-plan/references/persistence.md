# Persistence

| Situation | Result |
| --- | --- |
| no plan targets the same assumptions | create one |
| an open or collecting plan targets the same assumptions | update it |
| a done or cancelled plan targets the same assumptions | create one that lists it under `supersedes` |
| plan originates from an artifact | record that artifact under `source` |

Write a Markdown plan as `<slug>.md` at its location, the title in kebab-case. Relation values are project-relative paths or tracker ids.

## Location

Project memory's `backlog.md` says where work items and product artifacts live.

| Situation | Location |
| --- | --- |
| explicit target | use it |
| existing artifact | keep its support and path |
| a row of the `## Representation` table in the `backlog.md` memory file names the artifact | that support and native representation, once confirmed to exist |
| several targets remain | ask the user |
| `backlog.md` absent, or no row names the artifact | the default below; tell the user the default was used |

| Artifact | Default |
| --- | --- |
| research plan | `aidd_docs/backlog/research/` |

Markdown is the only support these skills write today. Naming another one is a project's own integration.
