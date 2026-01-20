# OWASP Top 10: Injection — Quick Reference

| Type | Example | Primary Fix |
| --- | --- | --- |
| SQL Injection | `OR 1=1` | Parameterized queries |
| NoSQL Injection | JSON operator abuse | Query allowlists |
| OS Command Injection | `; rm -rf` | Avoid shell, allowlists |
| Template Injection | SSTI | Safe templates |
