# Business Logic Flaws — Mid-Senior

1. How do you model a secure checkout workflow? — Server-side state machine with invariants.
2. How do you prevent double-spend in wallets? — Atomic transactions and idempotency keys.
3. How do you detect logic abuse in logs? — Track anomalies in sequence and frequency.
4. How do you prevent abuse of free trials? — Device or payment verification, rate limits.
5. How do you design safe discount logic? — Server-side computation, caps, auditing.
6. How do you secure multi-step KYC flows? — Session-bound state and step validation.
7. How do you mitigate timing-based order manipulation? — Locking and consistent reads.
8. How do you prevent referral fraud? — Fraud rules, uniqueness checks, and limits.
9. How do you secure promotions in distributed systems? — Central rule engine, consistent pricing.
10. How do you test business logic? — Abuse cases and adversarial test plans.
11. How do you enforce invariants across microservices? — Transactional boundaries and compensations.
12. How do you prevent API misuse that is valid but harmful? — Risk scoring and throttles.
13. How do you secure permissions in complex workflows? — State-dependent RBAC/ABAC.
14. How do you design safe approval flows? — Dual control and audit trails.
15. How do you handle partial failures in workflows? — Idempotent retries and reconciliation.
