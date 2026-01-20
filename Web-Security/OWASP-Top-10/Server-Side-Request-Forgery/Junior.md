# OWASP Top 10: Server-Side Request Forgery (SSRF) — Junior / Entry Level

1. What is SSRF? — Forcing a server to make requests to unintended targets.
2. Why is SSRF dangerous? — It can access internal services or metadata.
3. What is cloud metadata? — Internal endpoints with credentials.
4. What is an internal service? — Private network resources.
5. What is DNS rebinding? — Changing DNS to reach internal IPs.
6. What is URL allowlisting? — Restricting destinations to safe domains.
7. Why is URL validation hard? — URLs can be encoded or redirected.
8. What is a redirect-based SSRF? — Abuse of open redirects.
9. What is a file scheme SSRF? — Accessing local files via URL schemes.
10. What is a gopher scheme SSRF? — Using gopher to send raw requests.
11. What is a blind SSRF? — No response, but side effects exist.
12. What is an SSRF in image fetchers? — Fetching attacker-controlled URLs.
13. Why is IP allowlisting helpful? — Limits access to internal ranges.
14. What is a proxy SSRF? — Using the server as a proxy to other targets.
15. What is a SSRF via PDF generation? — Fetching remote content in server-side renderers.
