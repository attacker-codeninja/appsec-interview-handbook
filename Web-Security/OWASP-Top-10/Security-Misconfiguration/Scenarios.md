# OWASP Top 10: Security Misconfiguration — Scenario-Based

1. A production app is running in debug mode. What do you do? — Disable debug and rotate secrets.
2. A bucket becomes public due to a policy change. How do you respond? — Block access and audit.
3. An admin console is exposed on the internet. How do you fix? — Restrict access and add MFA.
4. A service uses wildcard CORS with credentials. What do you change? — Use explicit allowlists.
5. A container runs with default root user. How do you fix? — Run as non-root.
6. A web server exposes directory listings. What do you do? — Disable listing and review access.
7. An error page reveals stack traces. What do you do? — Use safe error pages.
8. A database is publicly reachable. How do you fix? — Move to private subnet and restrict SGs.
9. A config file with secrets is committed. How do you respond? — Rotate secrets and add scanning.
10. A CSP report shows unsafe inline scripts. What do you do? — Migrate to nonces.
11. A CI pipeline runs with admin cloud permissions. How do you fix? — Scope permissions.
12. A load balancer allows TLS 1.0. How do you fix? — Disable weak protocols.
13. A default API gateway key is still active. What do you do? — Rotate and revoke defaults.
14. An internal service has open metrics endpoints. How do you fix? — Add auth or network controls.
15. A server uses default SSH config. What do you improve? — Disable root login and use keys.
