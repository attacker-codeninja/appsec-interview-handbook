# Android Security — Mid-Senior

1. How do you secure exported components? — Restrict with permissions and intent filters.
2. How do you prevent intent hijacking? — Explicit intents and signature permissions.
3. How do you secure WebView? — Disable JS, use `addJavascriptInterface` carefully.
4. How do you implement device attestation? — Play Integrity with server validation.
5. How do you handle keystore key rotation? — Versioned keys and migration.
6. How do you detect repackaged apps? — Signature checks and integrity validation.
7. How do you protect deep links? — Verify app links and validate parameters.
8. How do you secure content providers? — Enforce permissions and validate queries.
9. How do you prevent sensitive data in logs? — Centralized logging policy and linting.
10. How do you handle encrypted storage? — Use EncryptedSharedPreferences/SQLCipher.
11. How do you implement secure backups? — Exclude sensitive data and encrypt.
12. How do you mitigate overlay attacks? — Detect overlays and use `FLAG_SECURE`.
13. How do you handle rooted device detection? — Combine signals; avoid blocking legitimate users.
14. How do you secure JNI/native code? — Validate inputs and harden builds.
15. How do you secure push token handling? — Store securely and rotate as needed.
