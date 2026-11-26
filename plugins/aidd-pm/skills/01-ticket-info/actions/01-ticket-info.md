# 01 - Ticket Info

Resolve the ticket identifier, query the configured ticketing tool, and display the relevant fields.

## Input

An optional ticket id or URL. When omitted, auto-detect it from the current branch name.

## Process

1. Resolve the ticketing tool and the ticket identifier per [tool-detection.md](../references/tool-detection.md).
2. Invoke the configured ticketing tool to fetch the ticket record.
3. Fill [ticket-template.md](../assets/ticket-template.md) from the queried record and render it for the user.

## Output

The ticket rendered per [ticket-template.md](../assets/ticket-template.md).

## Rules

- Every field the template defines matches the queried record, and the displayed URL opens the same ticket in the tracker.
