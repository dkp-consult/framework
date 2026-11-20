---
name: 08-three-amigos
description: Assesses an Epic or Story through one product, delivery, or quality lens, or reconciles three supplied reports, not for spawning or writing.
argument-hint: artifact | reports
---

# Three Amigos

```mermaid
flowchart LR
  target([Epic or Story]) --> assess["actions/01-assess.md"] --> report([one role report])
  reports([three role reports]) --> reconcile["actions/02-reconcile.md"] --> result([findings, conflicts, questions])
```

## Transversal rules

- Run one route per invocation.
- Never spawn, delegate, persist, or mutate.
- Treat roles as analytical lenses, not human authorities.
- Ground every finding and question in cited evidence and never invent a decision.
- Return proposals only, and let the caller decide what to do with them.
