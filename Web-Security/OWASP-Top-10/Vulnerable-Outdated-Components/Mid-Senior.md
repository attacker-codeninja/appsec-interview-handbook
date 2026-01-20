# OWASP Top 10: Vulnerable and Outdated Components — Mid / Senior Level

1. How do you integrate SCA into CI? — Scan on PRs and block critical issues.
2. How do you manage remediation at scale? — Prioritize by exploitability and exposure.
3. How do you reduce dependency sprawl? — Remove unused packages and consolidate.
4. How do you manage EOL migrations? — Plan upgrades and test compatibility.
5. How do you prevent dependency confusion? — Use private registries and namespaces.
6. How do you validate third-party packages? — Use allowlists and signed packages.
7. How do you manage SBOMs? — Generate per build and store in artifacts.
8. How do you handle container CVEs? — Rebuild images with patched bases.
9. How do you handle critical zero-days? — Hotfix, mitigations, and monitoring.
10. How do you keep lockfiles secure? — Review diffs and automate updates.
11. How do you monitor exploitability? — Use EPSS and vendor advisories.
12. How do you manage vendor libraries? — Review and update regularly.
13. How do you reduce false positives? — Map CVEs to usage context.
14. How do you secure build pipelines? — Verify sources and pin versions.
15. How do you enforce dependency policies? — Use policy-as-code in CI.
