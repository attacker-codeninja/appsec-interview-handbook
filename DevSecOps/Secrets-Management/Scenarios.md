# Secret Management — Scenarios

1. A secret is found in a public repo. What do you do? — Revoke, rotate, and investigate.
2. A vault outage blocks deployments. What do you do? — Use cached short-lived creds.
3. Developers store secrets in `.env` committed to repo. How do you fix? — Scanning and policy enforcement.
4. A long-lived API key is used by multiple services. How do you fix? — Split and scope keys.
5. A third-party vendor needs DB access. How do you provide it? — Short-lived, scoped credentials.
6. Secrets are leaking through error logs. How do you fix? — Redact and limit logging.
7. A service needs cross-cloud secrets. How do you manage? — Central vault or federation.
8. A compromised developer machine might have secrets. What do you do? — Rotate and revoke access.
9. You need to rotate TLS keys without downtime. How do you do it? — Overlapping certs and hot reload.
10. A CI job logs environment variables. How do you fix? — Mask secrets and remove logging.
11. A K8s secret is base64 only. What is the risk? — Not encrypted; use encryption at rest.
12. A mobile app uses a static API key. How do you fix? — Move to user-auth tokens.
13. A secret manager audit shows unusual access. What do you do? — Revoke and investigate.
14. A system uses shared SSH keys. How do you improve? — Use per-user keys and certs.
15. A new microservice needs secrets quickly. How do you provision? — Use templates and vault policies.
