# 02 - Slice

Find the smallest useful vertical slices within the confirmed scope.

## Input

The confirmed Story scope.

## Process

1. Apply [slicing](../references/slicing.md) to the user outcome.
2. Apply [relations](../references/relations.md) to known parents, dependencies, and blockers.
3. Remove or reclassify technical layers, broad outcomes, and unresolved questions.
4. Ask only when alternative slices change delivered value, and draft no Story until the user chooses.
5. Read [write](03-write.md).

## Output

An approved candidate list with value and known relations.

## Rules

- Each candidate names one observable user or stakeholder outcome.
- Every supported known relation is present, and none is invented.
- A completed source is no dependency unless it blocks delivery.
