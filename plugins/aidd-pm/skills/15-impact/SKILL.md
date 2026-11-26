---
name: 15-impact
description: Measures whether a released change moved its success signal against a frozen rule when preparing or judging it, not for acceptance or cost checks.
argument-hint: change | report
---

# Impact

```mermaid
flowchart LR
  change([change to arm]) --> arm["actions/01-arm.md"]
  arm -->|"change unidentified"| ask([one question asked])
  arm -->|"Epic not ready, no early arming asked"| notReady([arming waits for ready])
  arm -->|"another source chosen"| arm
  arm -->|"no success signal"| epic([signal owner offered])
  arm -->|"no source, manual refused"| noSource([Research plan offered])
  arm -->|"baseline export pending"| exportWait([export requested, arming waits])
  arm -->|"proposal rejected"| arm
  arm -->|"already released"| measure["actions/02-measure.md"]
  arm --> persist["actions/04-persist.md"]
  report([armed or measuring report]) --> measure
  report -->|"early armed, Epic now ready"| arm
  report -->|"cancel or new release date"| persist
  closed([judged or cancelled report]) -->|"new measurement"| measure
  unarmed([unarmed change]) --> measure
  measure -->|"no success signal"| epic
  measure -->|"no source, manual refused"| noSource
  measure -->|"window not over"| wait([end date reported])
  measure -->|"reading pending"| persist
  measure --> judge["actions/03-judge.md"]
  judge --> persist
  persist -->|"not authorized"| draft([draft shown])
  persist -->|"transition refused"| refused([status unchanged])
  persist -->|"armed"| armed([armed report with its follow-up])
  persist -->|"reading pending"| measuring([measuring report])
  persist -->|"cancelled"| cancelled([cancelled report])
  persist -->|"inconclusive"| research([Research plan offered])
  persist -->|"judged"| owner([verdict offered to the owner])
```

## Transversal rules

- Keep product and lifecycle decisions with the user.
- Separate evidence, decisions, and assumptions.
- Preserve source links and existing edits.
- Ask natural questions and never expose actions, references, or unchanged state.
- Require explicit approval or caller-provided bounded authority before any write.
- Freeze the signal, baseline, and decision rule before any post-release reading, refuse a later change, and record a departure as a deviation with the user's reason.
- Treat a movement as correlation, not causation, and always list the confounders.
- Never write into an Epic or a Story, and propose the result to its owner instead.
- Keep the follow-up of a measurement only in the report's `## Follow-up` section, never in another store, and schedule a reminder through the host only when the user asks.
- Read and write aggregated figures only, never a person's name, email, or customer identifier.
