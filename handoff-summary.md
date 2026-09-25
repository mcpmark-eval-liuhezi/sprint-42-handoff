# Sprint 42 Close-Out Handoff

Sprint 42 closes Friday. This summary hands the sprint over to the next support rotation and records the final status of every task in the Sprint 42 Tasks tracker.

## Final status per task

| Task | Assignee | Points | Status |
| --- | --- | --- | --- |
| Migrate auth tokens to vault | Dana Whitfield | 5 | Done |
| Retire the legacy CSV exporter | Marcus Chen | 3 | Backlog |
| Fix invoice PDF last-line bug | Marcus Chen | 3 | Blocked |
| Document webhook retry behavior | Alex Turner | 2 | Backlog |
| Upgrade Postgres to 16.4 | Priya Raman | 8 | Done |
| Investigate invoice PDF SKU overflow | Marcus Chen | 2 | Backlog |

## Close-out notes

- The vault migration landed this morning, so "Migrate auth tokens to vault" is closed out as Done.
- "Retire the legacy CSV exporter" will not make the deadline; it has been moved back to Backlog so the next rotation can pick it up.
- "Fix invoice PDF last-line bug" remains Blocked on the billing team.

## Known issues carried into next sprint

1. The invoice PDF renderer drops the last line item when a customer has more than 50 SKUs.
2. Webhook retries silently stop after the third failure and the ops runbook does not cover this yet.
