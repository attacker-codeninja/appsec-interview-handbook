# iOS Security — Scenarios

1. An app uses `NSAllowsArbitraryLoads`. How do you fix? — Remove and enforce ATS.
2. Users report deep link hijacking. What do you do? — Move to Universal Links.
3. A jailbroken device bypasses in-app purchases. How do you stop it? — Server-side receipt validation.
4. Tokens are found in backups. How do you fix? — Use `kSecAttrAccessibleWhenUnlockedThisDeviceOnly`.
5. A third-party SDK injects trackers. How do you respond? — Replace SDK and update privacy notices.
6. A WKWebView allows arbitrary navigation. How do you mitigate? — Restrict navigation with allowlists.
7. A crash report exposes PII. How do you fix? — Redact logs and reduce data.
8. Your app uses custom URL schemes for auth. How do you improve? — Use Universal Links with PKCE.
9. App Attest fails for some devices. How do you handle? — Graceful fallback and risk scoring.
10. A reverse engineer extracts API keys. What do you do? — Rotate keys and move to backend.
11. A dev build is shipped to production. What do you do? — Revoke and release fixed build.
12. A user claims account takeover via deep link. How do you investigate? — Validate link handling and logs.
13. ATS breaks a critical endpoint. What is your plan? — Stage migration and add scoped exceptions.
14. A jailbreak bypasses integrity checks. What do you change? — Add server-side controls.
15. A network proxy intercepts traffic. How do you detect? — Pinning and certificate validation.
