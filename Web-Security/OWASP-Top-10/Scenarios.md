# Web Application Security: OWASP Top 10 (2021/2024) — Scenarios

1. How would you secure a reporting endpoint that accepts flexible filters? — Validate inputs, parameterize queries, limit predicates.
2. If you must allow user-generated HTML, how do you prevent XSS? — HTML sanitization, CSP, strict allowlists.
3. You suspect SSRF to cloud metadata. What immediate fixes do you apply? — Block metadata IPs, enforce IMDSv2.
4. How would you protect an admin panel exposed to partners? — MFA, IP allowlists, fine-grained RBAC.
5. A legacy app stores passwords with MD5. How do you migrate? — Incremental re-hash on login, force reset.
6. A GraphQL API shows excessive data. How do you reduce exposure? — Query depth limits, field-level auth, persisted queries.
7. A bug bounty report shows token replay. How do you address it? — Rotate tokens, add nonce or token binding.
8. If you must support old browsers without CSP, what else helps? — Output encoding, strict input validation.
9. A single service uses multiple auth methods. How do you standardize? — Central auth gateway or shared auth library.
10. How do you handle access control for bulk export features? — Server-side checks per object and per scope.
11. A public bucket leaks PII. What is your response? — Block access, rotate keys, forensics, notify.
12. How do you secure multi-step workflows to avoid logic abuse? — Server-side state, step tokens, invariants.
13. An app uses third-party scripts. How do you reduce supply-chain risk? — SRI, CSP, pin versions, audit vendors.
14. How would you design logging for a high-traffic app? — Structured logs, sampling, correlation IDs.
15. A new feature uses webhooks. How do you secure it? — HMAC signatures, replay protection, allowlists.
