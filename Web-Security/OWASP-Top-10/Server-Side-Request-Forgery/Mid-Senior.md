# OWASP Top 10: Server-Side Request Forgery (SSRF) — Mid / Senior Level

1. How do you prevent SSRF in URL fetchers? — Allowlist domains and block internal IPs.
2. How do you protect cloud metadata? — Block metadata IPs and use IMDSv2.
3. How do you handle redirects safely? — Limit redirect chains and re-validate.
4. How do you mitigate DNS rebinding? — Resolve once and pin IP, then validate.
5. How do you implement egress controls? — Use firewall rules or proxy allowlists.
6. How do you secure webhook handlers? — Validate destinations and sign requests.
7. How do you detect SSRF attempts? — Monitor internal IP access and unusual egress.
8. How do you handle user-supplied URLs? — Parse strictly and block unsafe schemes.
9. How do you prevent SSRF in server-side rendering? — Block internal endpoints.
10. How do you protect internal services? — Require auth and restrict network access.
11. How do you deal with URL shorteners? — Expand and validate final destination.
12. How do you validate hostnames? — Use allowlists and DNS resolution checks.
13. How do you protect against SSRF in container environments? — Egress policies and network segmentation.
14. How do you prevent SSRF via file uploads? — Avoid fetching remote URLs.
15. How do you assess SSRF risk? — Identify all server-side fetchers.
