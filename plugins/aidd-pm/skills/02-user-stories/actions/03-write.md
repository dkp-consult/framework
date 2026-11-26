# 03 - Write

Write each approved candidate as a testable User Story.

## Input

The approved candidate list.

## Process

1. Fill the [User Story template](../assets/user-story-template.md) with the actor, need, and outcome.
2. Add sourced observable acceptance conditions.
   - Unknown behavior: ask or omit it.
   - Examples or Gherkin are clearer: use them.
3. Add known metadata from [relations](../references/relations.md).
4. Remove placeholders, every front matter key with no value, and `Cancellation` unless the status is `cancelled`.
5. Show the complete Story set, ask one open question on what should change, and stop until the user answers.
6. Fold the corrections, then read [assess](04-assess.md).

## Output

One Story draft per candidate.

## Rules

- This action writes nothing to any support.
- Each Story holds an actor, need, outcome, and at least one observable acceptance condition, all from the source or a confirmed decision.
- Acceptance holds product behavior only, and backlog relations stay metadata.
- Source metadata is absent unless backed by a stable id, URL, or project-relative path.
