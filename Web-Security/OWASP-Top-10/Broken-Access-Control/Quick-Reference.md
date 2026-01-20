# OWASP Top 10: Broken Access Control — Quick Reference

| Focus | Example | Primary Fix |
| --- | --- | --- |
| Object Access | IDOR/BOLA | Server-side authZ checks |
| Function Access | BFLA | Role and scope enforcement |
| Tenant Isolation | Cross-tenant access | Tenant scoping in queries |
| Session Abuse | Stolen tokens | Short TTL + rotation |
