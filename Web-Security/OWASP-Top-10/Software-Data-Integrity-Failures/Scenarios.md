# OWASP Top 10: Software and Data Integrity Failures — Scenario-Based

1. A malicious package appears in your dependency tree. What do you do? — Remove, rotate, and audit.
2. A build runner is compromised. How do you respond? — Rebuild runners and rotate secrets.
3. Your update server is compromised. What do you do? — Revoke keys and reissue signed updates.
4. A deserialization bug is found. How do you fix? — Switch to safe formats and allowlists.
5. A CI pipeline pulls unpinned actions. What do you change? — Pin to trusted versions.
6. A signed image fails verification in prod. What do you do? — Enforce signing in CI and investigate.
7. A developer modifies build scripts without review. How do you prevent? — Require reviews and checks.
8. A dependency confusion attack is suspected. What do you do? — Lock down registries and rename packages.
9. An attacker modifies config in Git. How do you detect? — Signed commits and audit alerts.
10. A key used for signing is leaked. What is your response? — Revoke and rotate signatures.
11. A package registry is unavailable. How do you reduce risk? — Mirror and pin dependencies.
12. A container registry is compromised. What do you do? — Rotate creds and verify images.
13. A data pipeline accepts unsigned events. How do you fix? — Sign and validate messages.
14. A third-party build action is deprecated. What do you do? — Replace and audit.
15. A build produces non-reproducible artifacts. How do you fix? — Use hermetic builds.
