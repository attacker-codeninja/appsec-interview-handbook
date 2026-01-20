# Infrastructure and Cloud Security (General) — Scenarios

1. A public S3 bucket leaks PII. What do you do? — Block public access, rotate creds, investigate.
2. A developer has admin access in production. How do you fix? — Remove and use just-in-time access.
3. An exposed security group allows SSH from the internet. What do you do? — Restrict to bastion and monitor.
4. A cloud API key is leaked. How do you respond? — Revoke and rotate.
5. A new region is enabled without controls. How do you fix? — Apply org policies and guardrails.
6. A logging pipeline is disabled. What do you do? — Restore and alert on changes.
7. A VPC peering allows unintended access. How do you fix? — Tighten routes and security groups.
8. A database is accessible publicly. How do you fix? — Private subnets and IAM auth.
9. A vendor needs access to a cloud account. How do you do it? — Use cross-account roles.
10. A new SaaS integrates with your cloud. What do you check? — OAuth scopes and audit logs.
11. A Kubernetes cluster uses node IAM roles. What do you do? — Use IRSA or workload identity.
12. A cloud function can access all buckets. What do you do? — Restrict bucket access.
13. A pipeline deploys without approval. How do you fix? — Add gates and policy checks.
14. A cloud service is end-of-life. What do you do? — Migrate and update controls.
15. An incident reveals missing logs. How do you respond? — Add logging policies and monitoring.
