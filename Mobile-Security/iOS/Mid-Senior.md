# iOS Security — Mid-Senior

1. How do you secure Keychain items? — Use proper accessibility and access control.
2. How do you enforce ATS without breaking legacy services? — Migrate endpoints and add targeted exceptions.
3. How do you detect jailbreak reliably? — Combine checks, avoid single indicators.
4. How do you secure WKWebView? — Disable JS where possible and restrict navigation.
5. How do you protect against URL scheme hijacking? — Use Universal Links and validation.
6. How do you handle Keychain migration? — Use key versions and re-encrypt on access.
7. How do you protect against runtime hooking? — Integrity checks and detection of tampering.
8. How do you store tokens securely? — Keychain with device-only access where possible.
9. How do you minimize permissions and entitlements? — Principle of least privilege.
10. How do you secure local data storage? — File protection and encryption.
11. How do you handle iOS privacy requirements? — Minimal collection and clear consent.
12. How do you handle device attestation? — App Attest with server validation.
13. How do you secure push notification payloads? — Avoid sensitive data, sign if needed.
14. How do you manage certificate pinning on iOS? — Pin public keys and rotate safely.
15. How do you test iOS apps for security? — Static analysis and dynamic testing with proxies.
