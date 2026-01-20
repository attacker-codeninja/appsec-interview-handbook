# Mobile Application Security (Common) — Mid-Senior

1. How do you design secure offline storage? — Encrypt at rest with per-user keys.
2. How do you handle secrets in mobile apps? — Use backend-mediated tokens, avoid hardcoding.
3. How do you implement certificate pinning safely? — Pin public keys, support rotations.
4. How do you mitigate rooted device abuse? — Attestation, risk scoring, limited access.
5. How do you detect app tampering? — Integrity checks, signature verification.
6. How do you protect against UI automation fraud? — Device signals, behavior analytics.
7. How do you handle secure inter-app communication? — Use explicit intents and permission checks.
8. How do you secure push notifications? — Avoid sensitive data in payloads.
9. How do you store tokens safely? — Keychain/Keystore with appropriate access control.
10. How do you secure background services? — Least privilege and strict IPC rules.
11. How do you handle mobile OS updates and security regressions? — Monitor OS versions and adjust policies.
12. How do you perform secure mobile code signing? — CI signing with protected keys.
13. How do you handle TLS interception by enterprise proxies? — Allow optional trust with user consent.
14. How do you test mobile apps for MITM? — Proxy testing with modified certs.
15. How do you integrate MASVS into SDLC? — Map controls to requirements and test cases.
