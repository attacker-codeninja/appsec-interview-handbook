# OWASP Top 10: Injection — Scenario-Based

1. A report endpoint accepts arbitrary filters. How do you secure it? — Allowlist fields and parameterize.
2. A legacy app builds SQL strings. How do you fix? — Migrate to parameterized queries.
3. A NoSQL API accepts JSON from clients. What do you change? — Validate schema and block operators.
4. An image converter uses shell commands. How do you secure it? — Use safe libraries and avoid shell.
5. A search endpoint needs advanced queries. How do you handle? — Use safe query DSL with allowlists.
6. A template engine renders user input. What do you do? — Sanitize and disable expression eval.
7. An LDAP search is vulnerable. How do you fix? — Escape input or use safe APIs.
8. A CSV export is vulnerable to formula injection. How do you fix? — Prefix dangerous chars.
9. A log pipeline breaks due to injection. How do you fix? — Sanitize log fields.
10. A batch job builds dynamic SQL. What do you do? — Use query builder and parameters.
11. A public API uses query params for sorting. How do you secure? — Allowlist sort fields.
12. A GraphQL resolver builds SQL. How do you fix? — Parameterize and enforce authZ.
13. A migration uses raw SQL from user input. How do you fix? — Remove user input from migrations.
14. A command injection PoC uses `;` separators. How do you mitigate? — Avoid shell, validate inputs.
15. A web app allows file path inputs. How do you secure? — Normalize and restrict paths.
