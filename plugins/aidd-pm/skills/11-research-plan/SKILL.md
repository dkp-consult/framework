---
name: 11-research-plan
description: Produces a research plan turning unproven assumptions into collectable evidence when the user prepares research, not for collecting or synthesizing.
argument-hint: idea | artifact | plan
---

# Research Plan

```mermaid
flowchart LR
  source([idea or artifact]) --> inventory["actions/01-inventory.md"]
  existing([existing plan]) --> persist["actions/05-persist.md"]
  inventory -->|"registry refused"| noRegistry([no registry])
  inventory -->|"only technical uncertainty"| spike([Spike offered])
  inventory --> qualify["actions/02-qualify.md"]
  qualify -->|"no decisive gap"| nothing([nothing to collect])
  qualify --> method["actions/03-method.md"]
  method --> kit["actions/04-kit.md"]
  kit --> persist
  kit -->|"method rejected"| method
  persist -->|"gaps or methods change"| qualify
  persist -->|"not authorized"| draft([draft shown])
  persist -->|"authorized"| done([research plan])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or caller-provided bounded authority before any write.
- Plan the collection only and never collect, synthesize, or conclude.
- Never write a person's name, email, or customer identifier to a file, and name a role or a segment instead.
