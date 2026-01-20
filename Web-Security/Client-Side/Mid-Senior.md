# Client-Side Attacks — Mid-Senior

1. How do you deploy a strict CSP without breaking apps? — Start with report-only, then tighten.
2. How do you prevent XSS in frameworks like React? — Avoid `dangerouslySetInnerHTML`, sanitize.
3. How do you secure postMessage communications? — Validate `origin` and message schema.
4. How do you reduce risk from third-party scripts? — SRI, CSP, sandboxed iframes.
5. How do you protect against clickjacking in legacy browsers? — X-Frame-Options.
6. How do you handle CSP nonces at scale? — Central middleware to generate and inject.
7. How do you detect DOM-based XSS in CI? — Use SAST rules and dynamic scanners.
8. How do you mitigate open redirect issues? — Allowlist destinations or use tokens.
9. How do you secure client-side routing? — Server-side access control is authoritative.
10. How do you prevent CSS injection? — Sanitize style inputs and disallow `url()`.
11. How do you handle third-party analytics safely? — Limit data, load via proxy.
12. How do you prevent token leakage in URLs? — Use POST or fragment, avoid query params.
13. How do you sandbox untrusted content? — Use iframes with `sandbox` attribute.
14. How do you mitigate DOM clobbering? — Use `document.getElementById`, avoid global IDs.
15. How do you handle window opener risks? — Set `rel="noopener"`.
