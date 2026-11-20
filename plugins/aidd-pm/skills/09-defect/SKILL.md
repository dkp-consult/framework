---
name: 09-defect
description: Produces or refines a backlog Defect when the user reports, assesses, links, orders, transitions, or verifies one, not for incidents or debugging.
argument-hint: report | defect
---

# Defect

```mermaid
flowchart LR
  source([report or Defect]) --> capture["actions/01-capture.md"]
  source -->|"already persisted"| finalize["actions/03-finalize.md"]
  capture --> assess["actions/02-assess.md"]
  assess -->|"revise"| capture
  assess --> finalize
  finalize -->|"revise"| capture
  finalize -->|"authorized"| done([Defect])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or bounded authority before any write, bounded authority being a grant from a calling skill or agent that names the exact write, never a user request.
- Record the mismatch and never diagnose or implement its fix.
