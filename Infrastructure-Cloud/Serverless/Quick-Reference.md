# Serverless Security — Quick Reference

| Risk | Example | Mitigation |
| --- | --- | --- |
| Over-permission | Wildcard IAM | Least privilege policies |
| Event Injection | Malicious payload | Validate event schema |
| Secrets | Env vars | Use secret stores |
| Dependency Risk | Vulnerable libs | SCA and pinned deps |
| Cold Start Logging | Sensitive logs | Redact logs |
