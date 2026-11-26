# 05 - Propose

Let the user decide the order, record that decision, and hand the changes to their owners.

## Input

The proposed ranking with its scores, evidence, and sensitivity.

## Process

1. Show the ranking, the scores, and their sensitivity, then ask for the decision and wait.
   - A value contested with new evidence: go straight to the last step.
   - A deviation from the proposed ranking: ask its reason and keep it.
2. Build the change set from the decided order per [change set](../references/change-set.md).
   - Done or cancelled items of the backlog: read them for a held order field per `change-set.md`.
   - Current order kept: build none.
   - No decided change touches an order field: handle it per `change-set.md`.
3. Show the decision and the change set, then ask for approval.
   - Not authorized: write no file and stop with the proposal shown.
4. Fill the [snapshot template](../assets/priorities-snapshot.md) with the decision and write it per [persistence](../references/persistence.md).
5. Read the snapshot back and report its path and the verification result.
6. Hand the change set to a backlog orchestration capability per [handoffs](../references/handoffs.md), with the snapshot as evidence and the authority granted.
   - No change set: stop on the snapshot.
   - No such capability installed: show the change set with each owner named and stop.
   - Entry on an external tracker: ask the product owner's authorization per `change-set.md`, and show the entry unhandled when refused.
7. Relay the receipts the owners return, a rejected change included.
   - Run offered by the capability owning an artifact: return the snapshot path to it per `handoffs.md`.
8. Read [score](03-score.md) when a value was contested with new evidence.

## Output

A decision snapshot path and the change set handed off, or the reason nothing was written.

## Rules

- Propose writes only the decision snapshot and never an item file.
- A held order field of a done or cancelled item is released in the same change set as the decided ranks, and no decided rank reuses its value.
