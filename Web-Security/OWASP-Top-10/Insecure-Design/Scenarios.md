# OWASP Top 10: Insecure Design — Scenario-Based

1. A checkout flow allows skipping payment. How do you fix? — Enforce server-side state transitions.
2. A product wants anonymous exports. How do you secure? — Require auth and limit scope.
3. A new feature adds public sharing links. How do you design safely? — Use short-lived, scoped tokens.
4. A team wants to store PII for analytics. What do you do? — Minimize collection and anonymize.
5. A workflow depends on client-side flags. How do you fix? — Validate state on server.
6. A new API lacks rate limiting. What is your response? — Add quotas and throttles.
7. A SaaS launches multi-tenant features. How do you design isolation? — Tenant IDs and data partitioning.
8. An admin panel is accessible to partners. How do you design controls? — Separate roles and strong MFA.
9. A system stores tokens in logs. How do you design logging? — Redact and tokenize sensitive fields.
10. A new integration requires webhooks. How do you design it? — HMAC signatures and replay protection.
11. A file upload feature is added. How do you secure? — Type allowlist and malware scanning.
12. A fraud risk is identified. How do you address in design? — Add risk scoring and limits.
13. A feature needs high availability. How do you design secure failover? — Secure config replication.
14. A legacy system cannot be patched. What design mitigations? — Compensating controls and isolation.
15. A new authentication method is added. How do you design safely? — Threat model and test flows.
