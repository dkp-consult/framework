# 01 - Inventory

Match each assumption to the sources the project declares.

## Input

An idea, or an artifact holding assumptions (Product Brief, Epic, impact result), by path or id.

## Process

1. Read the source and list the assumptions it rests on.
   - A bare idea: state the assumptions it implies and confirm them with the user.
   - Nothing identifies the idea: ask one question and wait.
2. Read the sources registry per [sources registry](../references/sources-registry.md).
   - Missing: propose one from what the project shows and fill the [sources template](../assets/sources.md) with one row per declared source.
   - Refused: stop without a coverage status and write no file.
3. Route each uncertainty about cost, feasibility, or design per [handoffs](../references/handoffs.md), listed apart with no coverage status.
   - Nothing else remains: stop on that offer.
4. Apply [coverage](../references/coverage.md) to each remaining assumption.
5. Read [qualify](02-qualify.md).

## Output

The assumptions, each with one coverage status and the source behind it.

## Rules

- Inventory changes no file except an approved sources registry.
