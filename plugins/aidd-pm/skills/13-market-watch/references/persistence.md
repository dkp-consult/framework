# Persistence

| Artifact | File at its location | Write |
| --- | --- | --- |
| market journal | `<competitor>.md`, the competitor in kebab-case | append only |
| insights registry | `<theme>.md`, the theme in kebab-case | add or update `market` rows only |

| Situation | Result |
| --- | --- |
| no journal for the competitor | create it from the [journal template](../assets/journal.md) |
| competitor with a new, changed, or removed observation | one dated entry with its rows, below the last one |
| competitor read with nothing new | one dated read line, so its last read advances |
| sources skipped | listed under the competitor's dated entry or line with the reason |
| competitor no longer watched | journal kept; one dated line states it |
| nothing new across the run | journal lines only, no theme file touched |
| no finding matters | journals written, no theme file touched |
| earlier entries | stay as written |
| run abandoned before approval | nothing written |

## Location

Project memory's `backlog.md` says where work items and product artifacts live.

| Situation | Location |
| --- | --- |
| explicit target | use it |
| existing artifact | keep its support and path |
| a row of the `## Representation` table in the `backlog.md` memory file names the artifact | that support and native representation, once confirmed to exist |
| that support holds no file, for a registry or a journal | ask the user; never split one across supports |
| several targets remain | ask the user |
| `backlog.md` absent, or no row names the artifact | the default below; tell the user the default was used |

| Artifact | Default |
| --- | --- |
| market journal | `aidd_docs/backlog/market/` |
| insights registry | `aidd_docs/backlog/insights/` |

Markdown is the only support these skills write today. Naming another one is a project's own integration.
