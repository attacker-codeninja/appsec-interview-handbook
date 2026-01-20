# iOS Security — Quick Reference

| Area | Risk | Mitigation |
| --- | --- | --- |
| Keychain | Weak access control | Use Keychain with access groups |
| ATS | Weak TLS | Enforce ATS, disallow exceptions |
| URL Schemes | Hijacking | Universal Links |
| Jailbreak | Runtime tampering | Attestation and checks |
| App Signing | Tampering | Verify code signature |
