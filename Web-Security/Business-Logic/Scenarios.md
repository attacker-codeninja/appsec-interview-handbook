# Business Logic Flaws — Scenarios

1. A user can cancel after shipment and get a refund. How do you fix? — Tie refund to delivery status.
2. An attacker buys negative quantities to gain credits. How do you prevent? — Validate min values server-side.
3. A coupon can be reused by editing the request. How do you fix? — Enforce per-user usage limits.
4. A user skips 2FA enrollment by navigating directly. How do you fix? — Require state for next steps.
5. Two concurrent checkouts oversell inventory. How do you prevent? — Lock inventory or use reservations.
6. A free trial can be reset by deleting cookies. How do you mitigate? — Server-side trial tracking.
7. A partner API allows bulk discounts. How do you prevent abuse? — Validate per-item and cap totals.
8. Referral bonuses are triggered with self-referrals. How do you stop it? — Identity and device checks.
9. A user can access premium features after downgrade. How do you fix? — Enforce entitlements at runtime.
10. A user can apply stacked promos. How do you control? — Rule engine with mutual exclusions.
11. A payout endpoint lacks idempotency. How do you fix? — Add idempotency keys and locks.
12. A loyalty points API allows transfers without authZ. How do you secure? — Verify owner on every transfer.
13. An attacker can change shipping address after payment. What do you do? — Lock address or require re-auth.
14. A confirmation email triggers an action without token. How do you fix? — Add signed, expiring tokens.
15. A user can call admin-only export via hidden UI. How do you fix? — Server-side authZ checks.
