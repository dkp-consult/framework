# Persistence

One Markdown file per theme, `<theme>.md` at the registry's location, the theme in kebab-case, with `type: insights` and `theme` in frontmatter.

| Situation | Result |
| --- | --- |
| scope matches an existing theme file | use that file |
| no theme file matches | create one from the [registry template](../assets/insights.md) |
| finding already in a `customer` row | append its evidence, update frequency and segments, recompute confidence |
| finding matches a `market` or `measured` row only | write a `customer` row naming that row in its Evidence as corroboration |
| row of origin `market` or `measured` | leave it as it is |
| no row matches | add one `customer` row |
| theme file without `## Customer runs` | append that section below the table |
| any write | add one line to `## Customer runs`; keep every other section, row, and line as it is |

| Column | Holds |
| --- | --- |
| Insight | the finding, worded per `rating.md` |
| Origin | `customer` |
| Evidence | each source link with its number of signals |
| Frequency | the total number of signals |
| Segment | the segments the signals come from |
| Confidence | `low`, `medium`, or `high` |
| Assumption | a link to each assumption it bears on, or empty |
| Effect | `supports`, `contradicts`, or `new` |

| Customer runs column | Holds |
| --- | --- |
| Date | the run date, `yyyy-mm-dd` |
| Scope | the theme, plan, assumption, or since the last run |
| Sources read | the declared sources read |
| Signals kept | their count |

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
| insights registry | `aidd_docs/backlog/insights/` |
| research plan | `aidd_docs/backlog/research/` |
| Product Brief | `aidd_docs/product/` |
| Epic | `aidd_docs/backlog/epics/` |

Markdown is the only support these skills write today. Naming another one is a project's own integration.
