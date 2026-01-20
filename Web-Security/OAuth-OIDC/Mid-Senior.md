# OAuth2 / OpenID Connect Security — Mid-Senior

1. How do you secure public clients on mobile? — Auth code + PKCE, no client secrets.
2. How do you prevent refresh token abuse? — Rotation, reuse detection, short TTL.
3. How do you validate JWTs correctly? — Verify signature, issuer, audience, exp, nbf.
4. How do you design scopes for least privilege? — Map scopes to API actions, avoid wildcards.
5. How do you secure multi-tenant OAuth? — Tenant-aware issuer and audience checks.
6. How do you handle logout for token-based systems? — Token revocation and session tracking.
7. How do you mitigate token leakage in SPAs? — Use BFF pattern or HTTP-only cookies.
8. How do you detect authorization code injection? — Strict redirect URI, PKCE, state.
9. How do you secure back-channel token exchange? — TLS, client authentication, mTLS.
10. How do you handle confidential vs public clients? — Secrets for confidential; PKCE for public.
11. How do you support multiple identity providers safely? — Per-IdP config, strict issuer validation.
12. What is the risk of `none` algorithm? — Allows unsigned tokens; must be disabled.
13. How do you handle clock skew for token validation? — Small leeway with strict max.
14. How do you secure token introspection? — Authenticate clients and limit access.
15. How do you build fine-grained authZ on top of OAuth? — Combine scopes with RBAC/ABAC.
