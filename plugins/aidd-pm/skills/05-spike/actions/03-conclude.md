# 03 - Conclude

Write the investigation outcome and reconnect it to the backlog.

## Input

The spike, its evidence, outcome status, and follow-up authority.

## Process

1. Complete the outcome and follow-up fields the evidence supports in the [spike template](../assets/spike-template.md).
2. Show the outcome and exact parent or backlog changes.
3. Ask for approval of the outcome and each related write, and wait: the request that started the run is not approval.
   - Only a calling skill or agent that names this exact write skips the wait, never the user's request.
   - Not authorized: return the proposal and leave parent and backlog content unchanged.
4. Apply the authorized changes through their owning supports.
5. Read the affected graph back and report the result.
   - After a write: the stable identity, changed fields as `before -> after`, affected relations, and the verification result.
   - A draft or no-write result: state that no persisted change occurred.
6. Apply [capabilities](../references/capabilities.md) to the follow-up when authorized.
7. Read [investigate](02-investigate.md) when the outcome is `inconclusive`.

## Output

A concluded Spike with coherent parent links and any authorized backlog update.

## Rules

- A resolved Spike never completes its parent automatically, and the parent's owner reassesses its readiness and planning fields.
