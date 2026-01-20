# Serverless Security — Scenarios

1. A function has admin IAM access. How do you fix? — Reduce permissions and audit.
2. An attacker floods API Gateway. How do you respond? — Rate limiting and WAF rules.
3. A function logs customer data. What do you do? — Redact and update policies.
4. A webhook triggers serverless workflows. How do you secure? — Signature validation.
5. A dependency has a critical CVE. What do you do? — Patch and redeploy quickly.
6. A function reads from S3 and writes to DB. What IAM policy do you set? — Limit to specific buckets and tables.
7. Events are replayed. How do you mitigate? — Idempotency and nonce checks.
8. You need to restrict outbound traffic. How do you do it? — VPC and egress rules.
9. A function stores secrets in code. How do you fix? — Move to secret manager.
10. A timeout causes partial processing. How do you handle? — Idempotent retries and DLQ.
11. A new region launch is needed. How do you secure it? — Replicate policies and logs.
12. A multi-tenant function accesses wrong tenant data. How do you fix? — Tenant checks and scoped tokens.
13. A step function fails on validation. How do you respond? — Validate earlier and add guardrails.
14. API keys are embedded in clients. How do you fix? — Move to user auth tokens.
15. A misconfigured trigger exposes internal data. What do you do? — Disable trigger and audit.
