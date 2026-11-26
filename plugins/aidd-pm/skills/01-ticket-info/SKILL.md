---
name: 01-ticket-info
description: Retrieves and shows a ticket from the configured tool when the user wants to see one, not for creating, commenting on, transitioning, or reassigning.
argument-hint: ticket
---

# Ticket Info

```mermaid
flowchart LR
  source([ticket id, or none]) --> ticketinfo["actions/01-ticket-info.md"]
  ticketinfo --> done([ticket displayed])
```
