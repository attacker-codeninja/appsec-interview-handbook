# OWASP Top 10: Security Logging and Monitoring Failures — Scenario-Based

1. An incident occurs but logs are missing. What do you do? — Restore logging and review coverage gaps.
2. Login failures spike overnight. How do you respond? — Investigate and block sources.
3. Logs contain full credit card numbers. What do you do? — Redact and rotate logs.
4. A service logs no authZ decisions. What do you change? — Add decision logging.
5. Alert fatigue is high. How do you fix? — Reduce noise and prioritize high-signal alerts.
6. A breach shows logs were tampered with. What do you do? — Move to immutable storage.
7. A new service ships without logging. What do you do? — Add logging requirements to SDLC.
8. A SIEM integration fails. What do you do? — Validate pipelines and add health checks.
9. A partner needs access to logs. How do you handle? — Least privilege and masking.
10. A zero-day hits your stack. How do you detect? — Add indicators and anomaly monitoring.
11. A DDoS overwhelms logging pipeline. What do you do? — Use sampling and rate controls.
12. Logs do not include user IDs. What do you change? — Add user context fields.
13. An attacker uses failed logins to enumerate users. How do you respond? — Add alerts and generic errors.
14. A privileged action lacks an audit record. What do you fix? — Ensure all admin actions are logged.
15. A log retention policy is too short. What do you do? — Extend retention and archive.
