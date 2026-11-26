---
name: 06-product-brief
description: Produces a concise Product Brief when the user frames or revisits a product opportunity and its validation, not for requirements, design, or planning.
argument-hint: idea | product
---

# Product Brief

```mermaid
flowchart LR
  source([idea or product]) --> frame["actions/01-frame.md"]
  frame --> discover["actions/02-discover.md"]
  discover -->|"ready or assumptions accepted"| shape["actions/04-shape.md"]
  discover -->|"visual helps"| visualize["actions/03-visualize.md"]
  visualize -->|"accepted or skipped"| shape
  shape -->|"evidence gap"| discover
  shape --> finalize["actions/05-finalize.md"]
  finalize -->|"learn more"| discover
  finalize -->|"change visual"| visualize
  finalize -->|"revise brief"| shape
  finalize -->|"authorized"| done([Product Brief])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or caller-provided bounded authority before any write.
- Frame the opportunity and never write requirements.
