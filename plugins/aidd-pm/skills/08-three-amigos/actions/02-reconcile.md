# 02 - Reconcile

Reconcile independent product, delivery, and quality assessments.

## Input

Exactly three reports, one per role, for the same Epic or Story snapshot.

## Process

1. Reject missing, duplicate-role, unevidenced, or different-snapshot reports.
   - Missing or duplicate role: return no result and identify the invalid roles.
   - Different snapshot: return no result and identify the target or revision mismatch.
2. Apply [reconciliation](../references/reconciliation.md).
3. Link every amendment and question to its source finding.
4. Return the result with its unresolved questions.

## Output

One refinement result with a verdict, findings, conflicts, amendments, and questions.

## Rules

- Never infer or request approval while a conflict stays unresolved.
