# Secret Management — Mid-Senior

1. How do you implement dynamic DB credentials? — Use vault to issue short-lived creds.
2. How do you handle rotation without downtime? — Dual secrets and phased rollout.
3. How do you manage secrets in Kubernetes? — Use sealed secrets or external vaults.
4. How do you secure CI secrets? — OIDC and ephemeral tokens.
5. How do you reduce secret sprawl? — Centralize and eliminate hardcoded usage.
6. How do you handle key escrow and recovery? — Secure backup with strict access.
7. How do you audit secret access? — Central logging and alerts.
8. How do you prevent secret exfiltration? — Egress controls and monitoring.
9. How do you manage tenant-specific secrets? — Namespacing and access controls.
10. How do you handle secrets in mobile apps? — Avoid embedding; use backend token exchange.
11. How do you protect TLS private keys? — Use KMS/HSM and tight ACLs.
12. How do you rotate OAuth client secrets? — Use overlapping credentials.
13. How do you handle developer access? — Just-in-time access and approvals.
14. How do you store secrets for serverless? — Use managed secret stores.
15. How do you manage secrets in IaC? — Use data sources or encrypted vars.
