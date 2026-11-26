---
name: 02-user-stories
description: Produces or refines ordered User Stories from a source when the user wants to slice, write, assess, order, or persist them, not for Epics or code.
argument-hint: request | epic
---

# User Stories

```mermaid
flowchart LR
  source([request, Product Brief, PRD, Epic, or Stories]) --> frame["actions/01-frame.md"]
  source -->|"already persisted"| finalize["actions/07-finalize.md"]
  frame --> slice["actions/02-slice.md"]
  slice --> write["actions/03-write.md"]
  write --> assess["actions/04-assess.md"]
  assess -->|"reshape"| slice
  assess --> estimation["actions/05-estimation.md"]
  estimation --> order["actions/06-order.md"]
  order --> finalize
  order -->|"reslice"| slice
  finalize -->|"revise"| write
  finalize -->|"authorized"| done([User Stories])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Draft only after actor, need, and outcome are explicit in the source or confirmed.
