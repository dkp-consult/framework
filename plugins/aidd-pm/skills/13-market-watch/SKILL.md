---
name: 13-market-watch
description: Tracks declared competitors with dated, cited observations when the user wants to run or resume a market watch, not for user feedback or one claim.
argument-hint: competitors | theme
---

# Market Watch

```mermaid
flowchart LR
  rivals([competitors]) --> scope["actions/01-scope.md"]
  focus([theme]) --> scope
  scope -->|"user feedback brought"| synthesis([synthesis offered])
  scope -->|"no watchlist, Research plan chosen"| plan([Research plan offered])
  scope -->|"no watchlist, none listed"| none([no watchlist])
  scope --> scan["actions/02-scan.md"]
  scan -->|"material refused"| refused([skips reported])
  scan -->|"no source readable"| unread([skips reported])
  scan --> compare["actions/03-compare.md"]
  compare --> persist["actions/04-persist.md"]
  persist -->|"observations or findings change"| compare
  persist -->|"not authorized"| draft([draft shown])
  persist -->|"authorized, nothing new"| quiet([nothing new reported])
  persist -->|"authorized"| done([journals and market insights])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Give every observation its URL and its date, and drop one that lacks either.
- Record what a competitor claims as announced, never as true.
- Read public pages only: no login, no paywall, and each site's terms respected.
- Summarize a fact in your own words and never copy page content.
- Never write a person's name, email, or customer identifier to a file, public review authors included, and name a role or a segment instead.
- Observe the market only and never recommend copying a feature or propose a solution.
- Never schedule a run, since the host wires the cadence in force.
