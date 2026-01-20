# OWASP Top 10: Cryptographic Failures — Quick Reference

| Focus | Example | Primary Fix |
| --- | --- | --- |
| Data in Transit | Weak TLS | Strong TLS config |
| Data at Rest | Plaintext storage | KMS + encryption |
| Passwords | Weak hashes | Argon2/bcrypt |
| Key Handling | Hardcoded keys | KMS/HSM + rotation |
