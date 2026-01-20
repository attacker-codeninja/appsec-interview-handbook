# API Security — Scenarios

1. How would you secure a public search API that powers a mobile app? — App attestation, rate limits, WAF.
2. An API accepts user-supplied URLs. How do you prevent SSRF? — Allowlist domains, block metadata IPs.
3. You discover a partner can access other tenants. How do you fix it? — Tenant-scoped authZ checks and logging.
4. How would you secure a GraphQL API used by multiple teams? — Persisted queries and field-level auth.
5. How do you handle API keys leaked in client apps? — Rotate keys, move to user-level auth.
6. Your API is behind a CDN. How do you maintain client IP for rate limits? — Use trusted headers and proxy rules.
7. A legacy endpoint lacks authZ but is used in production. What do you do? — Add checks, monitor, staged rollout.
8. A webhook endpoint is being spammed. How do you block? — Signature checks and IP allowlists.
9. How do you secure file download APIs? — Short-lived signed URLs and authZ validation.
10. A partner needs access to only one endpoint. How do you implement? — Fine-grained scope and separate client.
11. API errors leak stack traces. How do you fix? — Global error handler and safe error mapping.
12. A new API uses pagination tokens. How do you prevent tampering? — Signed or encrypted tokens.
13. An API supports bulk updates. How do you enforce per-item authZ? — Validate each item server-side.
14. Mobile apps call the API without auth. What is the risk? — Anyone can call it; move to token auth.
15. You want to expose analytics data externally. How do you reduce risk? — Aggregation, anonymization, and quotas.
