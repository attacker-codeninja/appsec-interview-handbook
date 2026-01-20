# Business Logic Flaws — Junior

1. What is a business logic flaw? — A vulnerability in intended flow, not code syntax.
2. Why are logic bugs hard to detect with scanners? — They require context of business rules.
3. What is a race condition in web apps? — Concurrent requests break invariants.
4. What is price tampering? — Modifying price fields in requests.
5. What is coupon abuse? — Reusing coupons beyond intended limits.
6. What is workflow bypass? — Skipping required steps in a process.
7. What is account enumeration? — Inferring valid users via responses.
8. What is rate limit abuse? — Circumventing limits with multiple accounts.
9. What is privilege escalation via business logic? — Using valid flows to gain unauthorized power.
10. What is trust on first use (TOFU) risk? — Accepting unverified state early.
11. What is IDOR in business flows? — Accessing another user’s data by altering IDs.
12. What is negative quantity abuse? — Using negative values to gain credits.
13. What is inventory race? — Overselling due to concurrent checkout.
14. What is refund abuse? — Triggering refunds without returning goods.
15. Why are consistent server validations important? — Client can be manipulated.
