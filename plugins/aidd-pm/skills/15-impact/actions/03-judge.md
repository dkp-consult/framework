# 03 - Judge

Apply the frozen rule to the reading and qualify how far the result can be trusted.

## Input

The reading, the baseline or its absence, and the decision rule from measure.

## Process

1. Derive the verdict from the reading per [judgment](../references/judgment.md).
2. Look for confounders inside the window per [confounders](../references/confounders.md), asking the user about what no source shows.
3. Set the confidence per `judgment.md`, then lower it per `confounders.md`.
4. Show the verdict, confidence, and confounders, ask the user for their decision, and wait.
5. Read [persist](04-persist.md).

## Output

A verdict, its confidence, the confounders, and any deviation.

## Rules

- Judge writes no file.
