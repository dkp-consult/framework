---
name: 07-epic
description: Produces or refines an outcome-based Epic when the user wants to frame, review, resume, or persist one, not for Product Briefs, Stories, or code.
argument-hint: request | epic
---

# Epic

```mermaid
flowchart LR
  source([request, Product Brief, PRD, or Epic]) --> shape["actions/01-shape.md"]
  source -->|"already persisted"| finalize["actions/03-finalize.md"]
  shape --> review["actions/02-review.md"]
  review -->|"revise"| shape
  review --> finalize
  finalize -->|"revise"| shape
  finalize -->|"authorized"| done([Epic])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Stay at outcome level and do not propose child slices or implementation.
