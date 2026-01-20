# Business Logic Flaws — Quick Reference

| Pattern | Example | Typical Fix |
| --- | --- | --- |
| Workflow Bypass | Skip payment step | Server-side state machine |
| Race Conditions | Double spend | Idempotency + locking |
| Price Manipulation | Client-controlled price | Server-side pricing |
| Abuse of Limits | Unlimited trials | Enforce quotas server-side |
| Trusting Client | Hidden fields | Recompute on server |
