# Mobile Application Security (Common) — Scenarios

1. A tester bypasses pinning. What do you change? — Pin to public keys, add integrity checks.
2. An APK is repackaged with malware. How do you respond? — Rotate keys, add attestation.
3. Users report tokens in logs. How do you fix? — Remove logging and rotate tokens.
4. A deep link opens without auth. How do you fix? — Validate session and inputs.
5. An attacker uses rooted devices for fraud. How do you mitigate? — Risk-based checks and limits.
6. The app must work offline with PII. How do you secure? — Encrypt with device-bound keys.
7. A device is lost. How do you protect data? — Remote wipe and short-lived tokens.
8. Your app is blocked by a corporate proxy due to pinning. What do you do? — Provide opt-in trust store.
9. QA reports sensitive data in backups. How do you fix? — Exclude from backups or encrypt.
10. A new OS version breaks keystore. How do you respond? — Feature flags and fallback logic.
11. A vendor SDK collects too much data. What do you do? — Reduce permissions or replace SDK.
12. Attackers scrape API endpoints from the app. How do you respond? — Enforce server-side authZ.
13. You must support older Android versions. How do you manage risk? — Limit features, enforce TLS.
14. A crash dump exposes secrets. How do you fix? — Redact and minimize crash data.
15. App integrity checks cause false positives. What do you adjust? — Calibrate risk thresholds.
