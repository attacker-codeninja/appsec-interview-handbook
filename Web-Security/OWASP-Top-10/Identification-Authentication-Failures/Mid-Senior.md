# OWASP Top 10: Identification and Authentication Failures — Mid / Senior Level

1. How do you implement secure MFA? — Use TOTP/WebAuthn and enforce for sensitive actions.
2. How do you mitigate credential stuffing? — MFA, rate limits, and breached-password checks.
3. How do you implement secure password reset? — Single-use tokens with short TTL.
4. How do you manage sessions safely? — Rotate tokens and invalidate on logout.
5. How do you validate JWTs? — Verify signature, issuer, audience, and expiry.
6. How do you prevent user enumeration? — Use generic error messages and rate limits.
7. How do you support passwordless auth? — Use WebAuthn or magic links with risk checks.
8. How do you enforce step-up auth? — Require re-auth for high-risk actions.
9. How do you handle device trust? — Use device binding and risk scoring.
10. How do you protect against session theft? — Use secure cookies and TLS.
11. How do you support SSO securely? — Use OIDC with PKCE and strict validation.
12. How do you monitor auth events? — Centralize logs and alert on anomalies.
13. How do you handle auth in mobile apps? — Use PKCE and avoid secrets.
14. How do you implement account recovery? — Verified channels and audit trails.
15. How do you enforce password rotation? — Only when risk-based or compromised.
