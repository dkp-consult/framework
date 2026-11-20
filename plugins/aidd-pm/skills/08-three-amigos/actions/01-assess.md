# 01 - Assess

Assess one Epic or Story through one requested lens.

## Input

One Epic or Story snapshot, its relevant sources, and `role: product|delivery|quality`.

## Process

1. Require exactly one supported role and one Epic or Story snapshot.
   - Missing or unknown role: return the supported roles and no assessment.
   - Missing or ambiguous target: return one target question and no assessment.
   - Unsupported artifact: return the Epic-or-Story requirement and no assessment.
2. Read only evidence relevant to the target and selected role.
3. Apply [assessment](../references/assessment.md).
4. Emit the report contract without changing any artifact.
   - No finding: return the inspected sources, `verdict: ready`, and `findings: []`.

## Output

One evidence-backed assessment report.
