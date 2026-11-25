# Persistence

One file per measurement: it carries the arming, when there was one, and the verdict.

| Situation | Result |
| --- | --- |
| no report exists for the change | create `<slug>.md` |
| an `armed` or `measuring` report exists for the change | update it |
| new release date on an `armed` report | update the release date, `window_end`, and the `## Follow-up` dates only |
| a `judged` or `cancelled` report exists and a new measurement is asked | create the next free suffix, `<slug>-2.md` then `<slug>-3.md`, listing the previous report under `supersedes` |
| any report | record the Epic or User Story under `source` |

A `judged` or `cancelled` report is never overwritten. Reports live at their location, the slug being the change title in kebab-case. Relation values are project-relative paths or tracker ids.

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
| impact report | `aidd_docs/backlog/impact/` |
| insights registry | `aidd_docs/backlog/insights/` |

Markdown is the only support these skills write today. Naming another one is a project's own integration.
