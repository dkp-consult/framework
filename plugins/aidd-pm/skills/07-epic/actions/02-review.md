# 02 - Review

Challenge whether the Epic is distinct, coherent, and ready for its next state.

## Input

The Epic draft.

## Output

A reviewed Epic and its next user decision.

## Process

1. **Compare.** Apply [persistence](../references/persistence.md) to find an existing match, overlap, or contradiction.
2. **Assess.** Apply [readiness](../references/readiness.md) to the complete draft.
3. **Challenge.** Test every claim against its source.
   - Outcome or need resting on an assumption with no evidence checkable before building: a finding for [handoffs](../references/handoffs.md).
4. **Route.** Let the user choose revision, finalization, or a capability from `handoffs.md`.
5. **Render.** Show a revised Epic or blocking finding; otherwise continue.

## Test

| Case | Pass |
| --- | --- |
| Quality gap | failed criterion maps to sourced evidence or one named gap |
| Existing match | update or reuse selected; identity preserved; no self-relation |
| Blocking uncertainty | no inferred claim; the capability handoffs names is offered |
| Outcome or need assumption stated, user silent | not accepted; the Epic does not pass readiness |
| Outcome or need resting on an unchecked assumption | Research plan offered; measuring after delivery only on the user's explicit acceptance of the risk |
| Review | no write |
| User output | no action, check, route, or unchanged-state label; a blocker ends with one open question |
