# API Security — Junior

1. What is API security? — Protecting endpoints, data, and identities exposed by APIs.
2. What is the difference between REST and GraphQL security concerns? — GraphQL enables over-fetching and complex queries.
3. What is API key auth and when is it insufficient? — Shared secrets; insufficient for user-level authZ.
4. What is a broken object level authorization (BOLA)? — Accessing objects by ID without permission checks.
5. What is BFLA (function level authZ)? — Calling admin functions without proper authZ.
6. Why is schema validation important? — Rejects invalid or malicious input early.
7. What is mass assignment? — Client sets fields that should be server-controlled.
8. Why are rate limits important? — Prevent brute force, scraping, and DoS.
9. What is API versioning and its security impact? — Old versions can remain vulnerable.
10. What is HMAC request signing? — Signing payloads to verify integrity and origin.
11. What is a replay attack in APIs? — Reusing a valid request to repeat actions.
12. What are idempotent methods? — GET/PUT should be safe or repeatable.
13. What is CORS and how does it affect APIs? — Controls browser access to API.
14. Why is TLS mandatory for APIs? — Protects tokens and data in transit.
15. What is token scope? — Limits access to specific resources or actions.
