# Threat Modeling (STRIDE / PASTA) — Scenarios

1. A new feature introduces a public webhook. How do you model it? — Map data flow, trust boundary, sign requests.
2. You are launching a multi-tenant SaaS. How do you model isolation risk? — Identify tenant boundaries and authZ.
3. A service uses third-party OAuth. What threats do you model? — Token misuse, redirect abuse.
4. A mobile app stores PII locally. What threats? — Device compromise and storage leakage.
5. A data lake integrates multiple sources. What threats? — Data poisoning and access control.
6. A high-traffic API faces DDoS. How do you model? — Availability threats and rate limits.
7. A CI pipeline builds production images. What threats? — Supply-chain and secrets exposure.
8. A feature uses generative AI. What new threats? — Prompt injection and data leakage.
9. A healthcare app handles PHI. How do you model compliance risk? — Regulatory and privacy threats.
10. A payment flow uses third-party processors. What threats? — Man-in-the-middle and fraud.
11. An internal admin tool is exposed to partners. What threats? — Privilege escalation and data access.
12. A device uses BLE. What threats? — Spoofing and replay.
13. A service uses serverless. What threats? — Event injection and IAM over-permission.
14. A legacy system cannot be patched. What mitigations? — Compensating controls and isolation.
15. A new logging pipeline is added. What threats? — Data leakage and tampering.
