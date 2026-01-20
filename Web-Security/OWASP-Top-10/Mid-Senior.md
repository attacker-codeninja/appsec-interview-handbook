# Web Application Security: OWASP Top 10 (2021/2024) — Mid-Senior

1. How do you prevent IDOR at scale? — Centralize authorization in services, use ABAC/RBAC, deny by default.
2. How would you redesign a system to resist injection across multiple data stores? — Use parameterized APIs, query builders, allowlists.
3. What architectural controls reduce SSRF? — Egress allowlists, metadata proxy, IMDSv2, network segmentation.
4. How do you secure JWT-based auth? — Short lifetimes, key rotation, strict alg allowlist, audience checks.
5. How do you enforce secure defaults in microservices? — Baseline configs, policy-as-code, golden templates.
6. How do you mitigate XSS in a modern SPA? — Output encoding, CSP, avoid dangerous DOM sinks.
7. How do you handle cryptographic migrations safely? — Dual write, staged rollout, key rotation, re-encryption jobs.
8. What controls prevent software supply-chain tampering? — Signed artifacts, provenance, protected branches.
9. How do you build effective detection for access control abuse? — Log authZ decisions with user, object, action, and outcome.
10. How do you prioritize OWASP findings with business context? — Risk-based scoring: exposure, impact, exploitability.
11. How do you prevent session hijacking in shared networks? — TLS everywhere, secure cookies, rotate on privilege change.
12. How do you handle multi-tenant data isolation? — Tenant IDs in every query, scoped indexes, row-level security.
13. How do you secure file uploads? — Allowlisted types, malware scanning, store outside web root.
14. How do you handle rate limiting without breaking legitimate traffic? — Adaptive limits, per-user keys, backoff.
15. How do you test for insecure design early? — Threat modeling and abuse case reviews.
