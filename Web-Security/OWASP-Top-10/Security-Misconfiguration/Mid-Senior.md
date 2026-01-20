# OWASP Top 10: Security Misconfiguration — Mid / Senior Level

1. How do you enforce secure configurations at scale? — Use IaC and policy-as-code.
2. How do you prevent drift from secure baselines? — Continuous configuration scanning.
3. How do you secure headers consistently? — Central middleware or gateway config.
4. How do you handle secrets in configs? — Use secret managers, not plaintext.
5. How do you harden container images? — Minimal base images and hardened defaults.
6. How do you manage cloud misconfigurations? — CSPM tools and guardrails.
7. How do you validate CORS safely? — Strict allowlists, avoid wildcard with credentials.
8. How do you handle feature flags in production? — Protect endpoints and limit exposure.
9. How do you prevent debug artifacts in prod? — CI checks and build profiles.
10. How do you secure admin endpoints? — Network isolation and strong auth.
11. How do you standardize TLS configs? — Use approved cipher suites and templates.
12. How do you prevent open storage buckets? — Default deny policies and automated checks.
13. How do you enforce secure file permissions? — Config management and audits.
14. How do you secure error handling? — Map to safe error responses.
15. How do you secure third-party services? — Harden integration settings and logs.
