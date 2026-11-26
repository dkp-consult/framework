# Insights registry

The insights registry, `<theme>.md` at its location per `persistence.md`, is a living register, one file per theme, shared by several capabilities. Frontmatter: `type: insights` and `theme: <theme>`.

| Column | Market row holds |
| --- | --- |
| Insight | the finding, stated as an observed market fact |
| Origin | `market` |
| Evidence | links to the journal files, the number of observations, and any corroborating or earlier row |
| Frequency | the share of the watchlist, such as `3 of 5 competitors` |
| Segment | the segment the competitors address, or `all` |
| Confidence | `low`, `medium`, or `high`, per the table below |
| Assumption | link to the assumption it touches, or empty |
| Effect | `supports`, `contradicts`, or `new`, per `comparison.md` |

| Confidence | When |
| --- | --- |
| `low` | one source, few occurrences, or self-reported only |
| `medium` | repeated within the market category, across several competitors |
| `high` | corroborated across at least two source categories; a linked `customer` or `measured` row brings the second |
| user need cap | a `market` row about a user need stays at most `medium` unless a linked `customer` or `measured` row corroborates it |

An announced offer is an observed public claim about that offer, never a self-reported signal.

| Situation | Handling |
| --- | --- |
| theme file missing | create it from the [insights template](../assets/insights.md), then add the rows |
| same finding already in a `market` row | dedup: append the evidence, update the frequency, recompute the confidence |
| same finding in a `customer` or `measured` row | corroboration: link that row in the Evidence of the market row, never edit it |
| rows of another origin | never written by this skill |
| section, row, or line this skill does not own, such as `## Customer runs` | kept as written |
