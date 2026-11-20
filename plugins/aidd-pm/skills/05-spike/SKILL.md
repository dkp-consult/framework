---
name: 05-spike
description: Frames, investigates, resumes, or concludes a spike when an uncertainty blocks estimation, feasibility, or design, not for general research or code.
argument-hint: question | spike
---

# Spike

```mermaid
flowchart LR
  source([question or Spike]) --> create["actions/01-create.md"]
  source -->|"already persisted"| investigate["actions/02-investigate.md"]
  create -->|"save for later"| done([Spike])
  create -->|"investigate now"| investigate
  investigate --> conclude["actions/03-conclude.md"]
  conclude -->|"inconclusive"| investigate
  conclude --> done
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Bound the question and never answer beyond its stop condition.
