---
name: 12-insights
description: Turns customer signals into evidence-rated insights when the user wants to synthesize tickets, interviews, surveys, or exports, not for market watch.
argument-hint: theme | plan | assumption | refresh
---

# Insights

```mermaid
flowchart LR
  theme([theme or product area]) --> scope["actions/01-scope.md"]
  plan([research plan]) --> scope
  assumption([assumption]) --> scope
  refresh([since the last run]) --> scope
  scope -->|"question to the user"| scope
  scope -->|"out of scope"| other([other capability offered])
  scope --> gather["actions/02-gather.md"]
  gather -->|"no registry, no material"| noRegistry([Research plan offered])
  gather -.->|"source unreadable"| exportAsked[/export request to the owner role/]
  gather -->|"no signal in scope"| gap([gap offered to Research plan])
  gather --> cluster["actions/03-cluster.md"]
  cluster --> confront["actions/04-confront.md"]
  confront --> persist["actions/05-persist.md"]
  persist -->|"regroup requested"| cluster
  persist -->|"not authorized"| draft([draft shown])
  persist -->|"authorized"| done([insights registry])
  persist -.->|"adaptation kept, no practices file"| practicesFile[/po-practices created/]
  persist -.->|"adaptation kept, practices file present"| learning[/learning capability offered/]
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Read what the sources hold and never generate, simulate, or complete a signal.
- Anonymize every verbatim and link to where it lives rather than copying it, so no person's name, email, or customer identifier reaches a file.
- Report what customers say and do and never propose a solution or a story.
