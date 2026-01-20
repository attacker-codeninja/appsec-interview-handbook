# OWASP Top 10: Cryptographic Failures — Scenario-Based

1. A legacy app stores passwords with MD5. How do you migrate? — Re-hash on login and force reset.
2. Your TLS config allows TLS 1.0. What do you do? — Disable weak protocols and ciphers.
3. A mobile app pins a certificate that is expiring. How do you rotate? — Pin public keys and stage overlap.
4. A database snapshot is unencrypted. What is your response? — Encrypt backups and rotate keys.
5. An API uses a shared HMAC key across environments. How do you fix? — Separate keys per env.
6. A service uses ECB mode. How do you fix? — Move to authenticated encryption (GCM).
7. You need to encrypt PII in logs. How do you do it? — Avoid logging or encrypt with keyed hashing.
8. A cert chain fails validation in prod. How do you fix? — Correct CA bundle and verify trust store.
9. A random token collision is observed. What do you do? — Increase entropy and use CSPRNG.
10. You must support a legacy client without modern TLS. How do you handle? — Isolate and add compensating controls.
11. A private key was exposed. What do you do? — Revoke, rotate, and re-issue certs.
12. A vendor stores data unencrypted. How do you respond? — Require encryption and contractual controls.
13. A migration to new hashing slows logins. What do you do? — Tune cost and scale resources.
14. A service uses JWTs with weak signing. What do you change? — Use strong algs and rotate keys.
15. A backup copy is found in a dev bucket. What do you do? — Remove, rotate, and harden policies.
