# Secret Management — Quick Reference

| Secret Type | Risk | Best Practice |
| --- | --- | --- |
| API Keys | Leakage | Rotate, scope, store in vault |
| DB Passwords | Privilege abuse | Use short-lived creds |
| TLS Private Keys | MITM | HSM or KMS protection |
| Tokens | Replay | Short TTL, rotation |
| SSH Keys | Lateral movement | Use cert-based auth |
