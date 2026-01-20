# OWASP Top 10: Broken Access Control — Mid / Senior Level

1. How do you centralize authorization in microservices? — Use a policy service or shared authZ library.
2. How do you prevent IDOR at scale? — Enforce tenant and ownership checks in data access layers.
3. How do you design least privilege roles? — Start minimal, review, and avoid wildcard permissions.
4. How do you handle access control in GraphQL? — Enforce authZ per resolver and per field.
5. How do you implement row-level security? — Use DB policies that enforce tenant/user filters.
6. How do you harden session management? — Short TTLs, rotation, and revocation lists.
7. How do you handle admin access safely? — Separate admin paths with strong MFA and audits.
8. How do you log authZ decisions? — Record user, resource, action, and result.
9. How do you prevent privilege creep? — Regular access reviews and automated policy tests.
10. How do you handle third-party access? — Scoped tokens and dedicated client credentials.
11. How do you protect access control in caches? — Key by user and permissions, avoid shared cache leakage.
12. How do you enforce step-up authentication? — Require re-auth for sensitive actions.
13. How do you protect bulk exports? — Per-object authZ and scope-limited exports.
14. How do you handle authZ in async jobs? — Carry user context and re-check permissions.
15. How do you test access control? — Automated tests for allow/deny cases and abuse paths.
