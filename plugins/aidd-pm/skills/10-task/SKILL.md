---
name: 10-task
description: Produces or refines a backlog Task for delivery work without independent user value when the user creates, links, orders, estimates, or completes one.
argument-hint: request | task
---

# Task

```mermaid
flowchart LR
  source([request or Task]) --> frame["actions/01-frame.md"]
  source -->|"already persisted"| finalize["actions/03-finalize.md"]
  frame --> review["actions/02-review.md"]
  review -->|"revise"| frame
  review --> finalize
  finalize -->|"revise"| frame
  finalize -->|"authorized"| done([Task])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Record delivery work and never plan or implement it.
