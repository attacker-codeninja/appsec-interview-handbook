# Web Application Security: OWASP Top 10 (2021/2024) — Quick Reference

| Category | Common Example | Core Mitigation |
| --- | --- | --- |
| Broken Access Control | IDOR | Enforce server-side authorization checks |
| Cryptographic Failures | Weak TLS, plaintext secrets | Strong TLS, proper key management |
| Injection | SQLi, NoSQLi, OS command | Parameterized queries, allowlists |
| Insecure Design | Missing threat modeling | Security requirements, design reviews |
| Security Misconfiguration | Default creds, verbose errors | Secure defaults, config hardening |
| Vulnerable and Outdated Components | Old libs | SBOM, patch management |
| Identification and Authentication Failures | Weak MFA | MFA, session management |
| Software and Data Integrity Failures | CI/CD tampering | Signed artifacts, pipeline hardening |
| Security Logging and Monitoring Failures | No alerts | Centralized logging, detection rules |
| Server-Side Request Forgery | Metadata access | Network egress controls, allowlists |
