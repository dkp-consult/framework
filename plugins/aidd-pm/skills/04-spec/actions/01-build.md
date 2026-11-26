# 01 - Build

Create a new spec from a need.

## Input

The need: the user's message, or the file it points to.

## Process

1. Read the need.
   - No outcome to name: ask one clarifying question and stop.
2. Fill [spec-template.md](../assets/spec-template.md) per [spec-content.md](../references/spec-content.md).
3. Show the spec and its open gaps, and wait for explicit approval: the request that started the run is not approval.
   - No approval: stop with no write.
4. Write it to `spec.md` in the feature folder `aidd_docs/tasks/<yyyy_mm>/<yyyy_mm_dd>_<slug>/` the need names, else in a new one dated with today's date, its slug naming the outcome: a month folder is never a feature folder.
5. Run [validate-spec.cjs](../scripts/validate-spec.cjs) on `spec.md`, fix, repeat until it passes.
6. Answer with its path and its open gaps as questions.

## Output

`spec.md`, or no write: one clarifying question, or a spec not approved.
