# OAuth2 / OpenID Connect Security — Scenarios

1. A SPA stores tokens in localStorage. How do you reduce risk? — Use HTTP-only cookies or BFF.
2. Your mobile app uses a client secret. What do you change? — Remove secret, use PKCE.
3. A partner needs long-lived access. How do you do it safely? — Short access tokens, refresh rotation.
4. Multiple apps share one OAuth client. What is the risk? — Scope and redirect abuse; split clients.
5. You see repeated refresh token reuse. What is your response? — Revoke tokens, alert, investigate.
6. How do you secure login with social providers? — Validate issuer, nonce, and `aud`.
7. An attacker can control redirect URIs. How do you fix? — Exact match allowlist and strict checks.
8. How do you protect an internal API that accepts JWTs? — Verify signature and audience; reject none.
9. You must allow native deep links. How do you reduce risk? — App-claimed links and PKCE.
10. How do you handle device token theft? — Bind tokens to device or use attestation.
11. Your IdP rotates signing keys. How do you handle it? — JWKS fetch with caching and rollover.
12. You want silent refresh in SPAs. What are the risks? — CSRF and iframe restrictions; use BFF.
13. How do you stop token replay across environments? — Environment-specific audience and issuer.
14. A user changes password. How do you invalidate sessions? — Revoke refresh tokens and rotate secrets.
15. A backend needs user identity. Which token do you use? — Use access token or verified ID token claims.
