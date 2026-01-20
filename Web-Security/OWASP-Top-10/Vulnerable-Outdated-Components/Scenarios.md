# OWASP Top 10: Vulnerable and Outdated Components — Scenario-Based

1. A critical CVE is announced in a core library. What do you do? — Patch, test, and deploy quickly.
2. A transitive dependency has a CVE. How do you fix? — Update root package or override version.
3. A legacy framework is unsupported. What is your plan? — Migrate and add compensating controls.
4. A malicious package is found in your build. How do you respond? — Remove, rotate, and audit.
5. A base image is outdated. What do you do? — Rebuild with a patched base.
6. A dependency update breaks the build. How do you handle? — Pin and schedule upgrade work.
7. A supply-chain attack hits a popular tool. What do you do? — Review SBOMs and rotate secrets.
8. A team adds a new package without review. How do you fix? — Add allowlist and review steps.
9. A CVE is marked low severity but internet-facing. What do you do? — Reassess risk and patch.
10. A client requires SBOMs. How do you provide? — Generate per release.
11. A package name is similar to internal libs. How do you prevent confusion? — Namespace and registry controls.
12. An internal tool bundles outdated libs. What do you do? — Update and scan regularly.
13. A vendor SDK is vulnerable. What do you do? — Patch or isolate and monitor.
14. A new dependency lacks maintenance. What do you do? — Evaluate alternatives.
15. A container image uses `latest`. How do you fix? — Use immutable tags.
