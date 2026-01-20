# OWASP Top 10: Server-Side Request Forgery (SSRF) — Scenario-Based

1. An image proxy fetches arbitrary URLs. How do you secure it? — Allowlist domains and block private IPs.
2. A PDF generator fetches external CSS. How do you fix? — Host assets locally or allowlist.
3. A webhook URL points to metadata IP. What do you do? — Block metadata access.
4. A user provides a shortened URL. How do you validate? — Expand and re-validate destination.
5. A DNS record changes after validation. How do you mitigate? — Resolve and pin IPs.
6. A service needs to fetch user avatars. How do you secure? — Use proxy with allowlists.
7. An SSRF PoC uses gopher. How do you fix? — Block non-HTTP schemes.
8. Internal admin panels are reachable. How do you fix? — Require auth and segment networks.
9. A cloud service uses IMDSv1. How do you fix? — Enforce IMDSv2 and block metadata IPs.
10. A URL parser allows `file://`. What do you do? — Block local file schemes.
11. You detect blind SSRF. How do you respond? — Add egress restrictions and logging.
12. A backend uses redirects in fetches. How do you secure? — Limit redirects and re-validate.
13. A crawler can access internal hosts. What do you do? — Run in isolated network.
14. A partner API calls your URL fetcher. How do you secure? — Restrict to allowlisted domains.
15. A service uses SSRF-prone libraries. How do you mitigate? — Patch and add network controls.
