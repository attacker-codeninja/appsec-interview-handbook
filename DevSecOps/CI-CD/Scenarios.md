# CI/CD Security (SAST/DAST/SCA Integration) — Scenarios

1. A secret leaks in CI logs. What do you do? — Rotate, scrub logs, add masking.
2. A critical CVE appears in a dependency. How do you respond? — Patch, hotfix, and notify.
3. Developers bypass security checks. How do you fix? — Enforce branch protection.
4. A CI runner is compromised. What is your response? — Rotate creds and rebuild runners.
5. DAST fails due to auth. How do you fix? — Add test accounts and auth helpers.
6. A third-party GitHub Action is hijacked. What do you do? — Pin versions and audit.
7. Builds are too slow due to scanning. How do you optimize? — Parallelize and cache.
8. A container image is deployed without scanning. What do you do? — Enforce admission policies.
9. A secrets scanner blocks a release. How do you handle? — Verify, rotate, re-run.
10. A developer disables a pipeline check. How do you prevent? — Lock workflows and review.
11. A package registry is unavailable. How do you reduce risk? — Mirror and pin.
12. A supply-chain attack hits your dependency. How do you detect? — SBOM and alerts.
13. CI uses long-lived tokens. How do you fix? — Use OIDC and short-lived tokens.
14. A DAST scan exposes staging data. How do you fix? — Use sanitized datasets.
15. A SAST rule flags too much. How do you tune? — Adjust rules and baseline.
