# OWASP Top 10: Cryptographic Failures — Mid / Senior Level

1. How do you choose a password hashing scheme? — Use Argon2id or bcrypt with proper cost.
2. How do you design key management? — Centralize in KMS with strict ACLs.
3. How do you rotate encryption keys without downtime? — Envelope encryption with staged rotation.
4. How do you enforce TLS across services? — TLS everywhere with strong ciphers and HSTS.
5. How do you validate certificates safely? — Trust chains, hostname checks, and pinning where needed.
6. How do you handle crypto migrations? — Dual-read and re-encrypt over time.
7. How do you protect backups? — Encrypt and restrict access.
8. How do you prevent key reuse? — Separate keys per purpose and environment.
9. How do you address cryptographic agility? — Abstract crypto to swap algorithms.
10. How do you securely generate randomness? — Use OS CSPRNG APIs.
11. How do you secure secrets in CI? — Use KMS-backed short-lived tokens.
12. How do you avoid crypto pitfalls in custom code? — Use vetted libraries only.
13. How do you secure API tokens? — Short TTL and secure signing keys.
14. How do you handle encryption at rest for databases? — Enable native encryption with KMS keys.
15. How do you prevent downgrade attacks? — Enforce TLS versions and HSTS.
