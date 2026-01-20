# Web Application Security: OWASP Top 10 (2021/2024) — Junior

1. What is Broken Access Control and why is it so common? — Missing server-side authorization checks, especially on object IDs.
2. Define IDOR and give a simple example. — Accessing `/user/123` without permission checks.
3. What is SQL injection and how do prepared statements prevent it? — SQLi injects code; prepared statements separate data from code.
4. What is XSS and what are the three main types? — Reflected, stored, and DOM-based XSS.
5. What is CSRF and when is it not a risk? — Cross-site request forgery; not a risk with same-site tokens or non-cookie auth.
6. What is SSRF? — Forcing a server to make requests to internal/metadata endpoints.
7. What is a security misconfiguration? — Insecure defaults like debug mode or open admin endpoints.
8. What is cryptographic failure in web apps? — Weak TLS, bad hashing, or poor key handling.
9. What is authentication failure? — Weak passwords, missing MFA, or bad session handling.
10. What is authorization vs authentication? — AuthN verifies identity; AuthZ verifies permissions.
11. What is a vulnerable component? — Outdated library with known CVEs.
12. What is an insecure design flaw? — Missing security controls from the architecture.
13. Why do logging and monitoring matter? — You cannot detect or respond to attacks.
14. What is session fixation? — Forcing a user to use a known session ID.
15. What is content security policy (CSP)? — A browser policy to reduce XSS impact.
