# Android Security — Scenarios

1. A WebView uses `addJavascriptInterface` with sensitive methods. How do you fix? — Remove or restrict interface.
2. A third-party SDK requests many permissions. What do you do? — Minimize or replace SDK.
3. Users can access your exported Activity and bypass login. How do you fix? — Add auth checks and restrict export.
4. An APK is modified and distributed. How do you respond? — Revoke, alert, and add integrity checks.
5. A root detection causes false positives. How do you handle? — Use risk scoring and graceful degradation.
6. Sensitive data is backed up to Google Drive. How do you fix? — Exclude or encrypt data.
7. An Intent is intercepted by another app. How do you mitigate? — Use explicit intents and permissions.
8. An app link is hijacked by another app. How do you fix? — Verify app links and set defaults.
9. A crash log contains tokens. What do you do? — Redact logs and rotate tokens.
10. Your app uses HTTP for analytics. How do you fix? — Enforce HTTPS in `networkSecurityConfig`.
11. A debug build was shipped to production. What do you do? — Revoke, release fixed build.
12. App uses weak TLS ciphers on old devices. How do you handle? — Update TLS stack and enforce.
13. A content provider leaks user data. How do you fix? — Tighten permissions and validate inputs.
14. A rooted device uses automation to farm rewards. What do you do? — Add fraud controls and limits.
15. App signing key was exposed. What is your response? — Rotate keys and notify users.
