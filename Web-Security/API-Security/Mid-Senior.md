# API Security — Mid-Senior

1. How do you design object-level authZ checks across services? — Central policy service or shared library.
2. How do you prevent mass assignment in large APIs? — Explicit allowlists per endpoint.
3. How do you secure GraphQL against complex queries? — Depth limits, cost analysis, persisted queries.
4. How do you handle API auth for B2B integrations? — Mutual TLS or signed requests plus scoped tokens.
5. How do you detect abuse patterns in APIs? — Anomaly detection on per-user/request metrics.
6. How do you manage API secrets rotation? — Short-lived tokens, automatic rotation and revocation.
7. How do you enforce least privilege with OAuth scopes? — Granular scopes mapped to endpoints.
8. How do you secure webhooks? — HMAC signatures, timestamps, and allowlists.
9. How do you handle multi-tenant isolation in APIs? — Tenant-aware queries, row-level security.
10. How do you implement consistent error responses without leaking details? — Standard error schema and safe messages.
11. How do you protect APIs from SSRF? — Validate URLs, restrict egress, resolve DNS safely.
12. What is API schema drift and how do you control it? — Contract tests, schema registry.
13. How do you prevent parameter pollution? — Reject duplicates or define precedence rules.
14. How do you secure admin-only APIs? — Dedicated authz policies and network isolation.
15. How do you handle async API actions securely? — Signed job tokens, status endpoints with authZ.
