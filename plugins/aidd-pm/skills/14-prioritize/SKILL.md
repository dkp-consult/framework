---
name: 14-prioritize
description: Ranks one backlog by the recorded method when the user wants to choose a method, score items, or see what flips the order, not for sibling Stories.
argument-hint: backlog | items | criteria
---

# Prioritize

```mermaid
flowchart LR
  source([backlog or items]) --> method["actions/01-method.md"]
  criteria([criteria]) --> method
  method -->|"Stories of one parent"| storyOwner([User Story owner offered])
  method -->|"method not recorded"| noScore([no score])
  method -->|"criteria only"| recorded([method recorded])
  method --> gather["actions/02-gather.md"]
  gather -->|"no snapshot: full run"| score["actions/03-score.md"]
  gather -->|"latest snapshot: changes only"| score
  score -->|"answer off the scale: asked again"| score
  score --> rank["actions/04-rank.md"]
  rank --> propose["actions/05-propose.md"]
  gather -->|"collect first"| research([Research plan offered])
  rank -->|"collect first"| research
  propose -->|"value contested"| score
  propose -->|"not authorized"| draft([proposal shown])
  propose -->|"current order kept or no order field touched"| snapshot([decision snapshot])
  propose -->|"no orchestration installed"| shown([change set shown])
  propose -->|"tracker change not authorized"| shown
  propose -->|"authorized"| done([change set handed off])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or caller-provided bounded authority before any write.
- Never propose a criterion value of your own: a criterion without mapped evidence takes the product owner's assessment, asked and flagged as a user assumption, or stays `unknown`.
- Propose a ranking and never decide it.
- Never write an order or priority field, since each artifact owner writes its own.
- Show every score with its sensitivity.
- Never write a person's name, email, or customer identifier to a file, and name a role or a segment instead.
