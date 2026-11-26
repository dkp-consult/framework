---
name: 03-prd
description: Generates a PRD from a need, idea, or brainstorm, confirmed before save, when the user wants to draft one, not for user stories or a technical plan.
argument-hint: need | brainstorm
---

# PRD

```mermaid
flowchart LR
  source([feature description, optionally with user stories]) --> draft["actions/01-draft.md"]
  draft --> finalize["actions/02-finalize.md"]
  finalize --> done([saved PRD])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or caller-provided bounded authority before any write.
- State what and why, never a technical plan or user stories.
