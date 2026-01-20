# OWASP Top 10: Injection — Mid / Senior Level

1. How do you eliminate injection across services? — Use parameterized APIs and query builders.
2. How do you handle dynamic filters safely? — Allowlist fields and operators.
3. How do you secure search features? — Use full-text engines with safe APIs.
4. How do you mitigate command injection in file processing? — Avoid shells, use safe libs.
5. How do you prevent template injection? — Use logic-less templates and sandboxed renderers.
6. How do you validate JSON inputs for NoSQL? — Reject operators and enforce schema.
7. How do you implement defense in depth for SQLi? — Param queries, least privilege, WAF.
8. How do you handle ORMs safely? — Avoid raw queries and validate inputs.
9. How do you test for injection in CI? — SAST rules and targeted DAST.
10. How do you limit damage of an injection? — DB role scoping and read-only replicas.
11. How do you secure stored procedures? — Use parameters and avoid dynamic SQL.
12. How do you detect injection attempts in logs? — Pattern-based detection and alerting.
13. How do you handle multi-tenant queries? — Always include tenant filters in queries.
14. How do you avoid query parameter pollution? — Define precedence and reject duplicates.
15. How do you secure file path inputs? — Normalize and allowlist directories.
