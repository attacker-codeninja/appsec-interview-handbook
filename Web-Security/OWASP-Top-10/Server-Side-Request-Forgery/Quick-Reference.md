# OWASP Top 10: Server-Side Request Forgery (SSRF) — Quick Reference

| Vector | Example | Primary Fix |
| --- | --- | --- |
| Metadata | IMDS access | Block metadata IPs |
| Internal Services | Private URLs | Egress allowlists |
| Redirects | Open redirect SSRF | Restrict redirects |
| DNS Rebinding | Host change | Resolve and pin IP |
