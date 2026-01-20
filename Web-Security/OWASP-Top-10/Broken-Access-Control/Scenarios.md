# OWASP Top 10: Broken Access Control — Scenario-Based

1. A user accesses another tenant's invoice by ID. How do you fix it? — Enforce tenant-scoped queries and authZ.
2. A partner integration needs read-only access. What do you do? — Issue scoped tokens with read-only permissions.
3. Users can enumerate accounts by error messages. How do you fix? — Use generic errors and rate limits.
4. An admin endpoint is publicly reachable. What do you change? — Restrict via network controls and MFA.
5. A user keeps access after role downgrade. How do you fix? — Recompute claims and invalidate sessions.
6. Bulk export exposes data to unauthorized users. How do you secure? — Filter by authZ per record.
7. A frontend hides a button but API still works. How do you fix? — Enforce authZ server-side.
8. A token leaked in URL logs. What is your response? — Revoke tokens and move to headers.
9. Support staff need time-bound access. How do you implement? — Just-in-time roles with expiry.
10. A single service supports multiple auth types. How do you standardize? — Centralize authZ checks.
11. An API uses only API keys for user actions. How do you fix? — Use user-bound tokens.
12. A SaaS offers cross-account sharing. How do you secure? — Explicit sharing rules and audit trails.
13. A user can access deleted resources. What do you do? — Enforce soft-delete filters in authZ.
14. A service trusts client-sent roles. How do you fix? — Derive roles from server-side claims.
15. A password reset link works twice. How do you fix? — Make tokens single-use and short-lived.
