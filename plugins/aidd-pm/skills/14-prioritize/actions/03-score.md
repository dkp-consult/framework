# 03 - Score

Value each criterion from its evidence, then score each item.

## Input

The evidence lines per item and criterion, or a contested value with new evidence.

## Process

1. Set each criterion value on its scale per [scoring](../references/scoring.md), keeping carried values as they are.
   - A value the user contests with new evidence: recompute that criterion only.
2. Ask the product owner, in one batched question, every value the evidence does not set and no snapshot carries, need levels included, and wait.
   - Answer off the recorded scale: handle it per `scoring.md` and wait.
   - No answer for a criterion: it stays `unknown`.
3. Set effort as total cost per `scoring.md`.
4. Flag every value resting on a `low` row or on the user's own statement.
5. Apply the method formula, a range where a criterion is `unknown`.
6. Rate each score's confidence and show its ceiling per `scoring.md`.
7. Read [rank](04-rank.md).

## Output

Per item: each criterion value with its citation or `unknown`, the score, and its confidence.

## Rules

- Score writes no file.
