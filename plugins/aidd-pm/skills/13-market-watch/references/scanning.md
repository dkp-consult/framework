# Scanning

| Mode | When | Material |
| --- | --- | --- |
| web | source access `web` and the host can read web pages, or access `mcp` or `cli` through the declared tool | the agent reads each page |
| manual | no web reading ability, or source access `export` or `manual` | the user pastes text or supplies an export |

| Source type | Look for |
| --- | --- |
| changelog | releases, capabilities, deprecations |
| pricing | plans, prices, limits, free tier, trial |
| docs | capabilities documented, integrations, supported platforms |
| public reviews | recurring praise and complaints, the reviewer segment when stated |

| Source state | Result |
| --- | --- |
| readable within the transversal rules | read |
| reading it would break a transversal rule | skipped, reason reported |
| unreachable | skipped, reason reported; its last read date stays, so the next run covers the gap |
| access `none` | skipped, the owner role named |

| Observation field | Holds |
| --- | --- |
| Competitor | the company or product as the watchlist names it |
| Date | the date shown on the page, else the date it was read; for pasted material, the date it carries |
| URL | the page the fact comes from |
| Observation | one fact in one sentence |
| Theme | the insights theme it touches, or none |

Since the last read of a source, read only what is dated after it; on a page without dates, compare its whole current state.
