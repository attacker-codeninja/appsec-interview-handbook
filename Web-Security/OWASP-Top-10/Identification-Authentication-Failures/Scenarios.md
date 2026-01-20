# OWASP Top 10: Identification and Authentication Failures — Scenario-Based

1. A password reset link can be reused. How do you fix? — Make tokens single-use and short-lived.
2. Users can enumerate accounts by login errors. What do you do? — Use generic responses.
3. An attacker replays a session token. How do you mitigate? — Rotate tokens and bind to device.
4. A mobile app uses a client secret. What do you change? — Remove secret and use PKCE.
5. A login endpoint is being brute forced. What do you do? — Rate limit and add MFA.
6. A user changes password but sessions stay active. How do you fix? — Invalidate existing sessions.
7. A new SSO provider is added. How do you secure it? — Validate issuer and audience.
8. A phishing campaign targets users. What mitigations? — MFA and phishing-resistant factors.
9. A legacy app stores passwords in SHA1. What do you do? — Migrate to bcrypt/Argon2.
10. An admin account lacks MFA. How do you fix? — Enforce MFA and alerts.
11. A token is stored in localStorage. How do you improve? — Use HttpOnly cookies or BFF.
12. Account recovery uses security questions. How do you improve? — Use verified email/SMS.
13. An API returns tokens in URLs. How do you fix? — Move to headers or cookies.
14. A session stays alive forever. How do you fix? — Add idle and absolute timeouts.
15. A service supports both SSO and local login. How do you secure? — Consistent policies and MFA.
