# Client-Side Attacks — Quick Reference

| Attack | Example | Mitigation |
| --- | --- | --- |
| XSS | Script injection | Output encoding, CSP |
| Clickjacking | UI redress | `X-Frame-Options`, CSP frame-ancestors |
| CSP Bypass | Inline script | Nonces and strict CSP |
| DOM Clobbering | Element ID override | Safe DOM APIs |
| Supply Chain | Malicious JS | SRI, pin versions |
