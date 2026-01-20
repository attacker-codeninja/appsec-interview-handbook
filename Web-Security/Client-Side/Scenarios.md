# Client-Side Attacks — Scenarios

1. A marketing script causes XSS. How do you respond? — Remove script, rotate tokens, add CSP.
2. A legacy app uses inline scripts. How do you add CSP? — Migrate to nonces and external files.
3. A partner widget runs in your page. How do you isolate it? — Sandbox iframe, restrict postMessage.
4. A phishing report cites your open redirect. How do you fix? — Allowlist or remove redirect.
5. A DOM XSS bug occurs only in a specific browser. How do you test? — Browser-specific security testing.
6. You need to embed third-party content. How do you secure? — Use iframe with `sandbox` and CSP.
7. Users copy URLs with tokens in query params. How do you fix? — Move tokens to headers.
8. An extension changes your checkout flow. What can you do? — Detect tampering and alert users.
9. A UI overlay causes unintended clicks. How do you mitigate? — Frame busting and UI integrity checks.
10. A malicious service worker is installed. How do you respond? — Revoke, update, clear SW.
11. A CSP report shows violations from ads. What do you do? — Adjust policy or remove ads.
12. A SPA stores JWTs in localStorage. How do you improve? — Use HTTP-only cookies or BFF.
13. A frontend app exposes secrets in source. How do you fix? — Remove secrets, rotate, use server.
14. Users report tabnabbing. How do you fix? — Add `rel="noopener noreferrer"`.
15. A support chat widget is compromised. How do you respond? — Kill switch, audit vendor, add SRI.
