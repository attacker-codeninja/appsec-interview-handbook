# OAuth2 / OpenID Connect Security — Quick Reference

| Flow | Use Case | Common Risk |
| --- | --- | --- |
| Authorization Code + PKCE | Public clients (mobile/web) | Missing PKCE or state |
| Client Credentials | Service-to-service | Over-broad scopes |
| Implicit (deprecated) | Legacy SPAs | Token leakage |
| Refresh Token | Long-lived sessions | Token theft and replay |
