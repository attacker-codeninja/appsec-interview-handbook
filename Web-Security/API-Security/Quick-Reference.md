# API Security — Quick Reference

| Control | Why It Matters | Typical Mistake |
| --- | --- | --- |
| AuthN/AuthZ | Prevents unauthorized access | Only checking authN, not authZ |
| Rate Limiting | Blocks abuse | Global limits without user context |
| Schema Validation | Stops injection and logic abuse | Accepting extra fields silently |
| Least Privilege | Reduces blast radius | Over-broad scopes |
| Logging | Detects abuse | Missing request context |
