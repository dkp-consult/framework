# 01 - Create

Qualify and persist an open spike without forcing investigation.

## Input

A question, related context, and any supplied route or authority.

## Process

1. Apply [capabilities](../references/capabilities.md) when the question or decision is unclear.
2. Apply [qualification](../references/qualification.md).
3. Apply [persistence](../references/persistence.md) and follow its result.
4. Resolve `save for later` or `investigate now`.
   - No route: ask for the choice and create no Spike.
5. Fill the [spike template](../assets/spike-template.md) fields the evidence supports, and [relations](../references/relations.md).
   - A keep-open Spike: stop after `Bounds` and omit `Investigation`, `Outcome`, `Follow-up`, and `Cancellation`.
   - A replaced Spike: record its cancellation and replacement under `Outcome` and `Follow-up`.
6. Show the Spike draft, its status, and any previous cancellation, ask for approval, and wait: neither the route nor the request that started the run is approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - No approval: create no Spike.
7. Write the approved Spike per `persistence.md`.
8. Read the affected graph back and report the result.
   - After a write: the stable identity, changed fields as `before -> after`, affected relations, and the verification result.
   - A draft or no-write result: state that no persisted change occurred.
9. Read [investigate](02-investigate.md) when the route is `investigate now`.

## Output

A spike reference, or the reason no spike is needed.

## Rules

- A missing question, decision, or authority creates no Spike.
- A Markdown Spike leaves no metadata field empty and keeps status and relation fields out of the body.
