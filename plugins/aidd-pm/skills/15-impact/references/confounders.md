# Confounders

Anything else inside the window that could move the same signal.

| Confounder | Where to look |
| --- | --- |
| another release touching the same journey or signal | backlog items completed in the window, release notes, version tags |
| seasonality | the same period a year earlier when the source holds it, else the user |
| marketing campaign, promotion, or price change | the user, then the `sales` or `billing` source |
| incident or outage | the user, then the `support` source |
| change in tracking or in the signal's definition | the `analytics` source, then the user |
| sample too small to tell a movement from noise | the reading itself |

| Finding | Effect |
| --- | --- |
| a confounder that can move the signal | listed with where it was found; confidence one level lower |
| a confounder that can explain the whole movement | verdict `inconclusive` |
| tracking or definition changed during the window | verdict `inconclusive` unless the reading can be corrected |
| nothing found | `none found`, with the places checked |
