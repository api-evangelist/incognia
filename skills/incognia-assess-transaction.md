---
name: Assess a login or payment transaction
description: Get a real-time risk verdict for a login or payment event using Incognia.
api: openapi/incognia-openapi-original.yml
operations: [createToken, registerTransaction]
---

# Assess a login or payment transaction

Use this at login or checkout to detect account takeover and payment fraud.

## Auth (operation: createToken)
Exchange `client_id`/`client_secret` (HTTP Basic) at `POST /v2/token` for a bearer token; send `Authorization: Bearer <access_token>` on the call below.

## Assess the transaction (operation: registerTransaction)
1. `POST /v2/authentication/transactions` with `type` set to `login` or `payment` and an `account_id`.
2. Provide device context via `installation_id` (mobile) or `request_token` (web); add `location`, `app_version`, and `device_os` when available.
3. For payments, include `payment_value` (`amount`, `currency`), `payment_methods[]`, and `addresses[]` (shipping/billing/home).
4. Read `risk_assessment` (`low_risk` / `high_risk` / `unknown_risk`), `reasons[]`, `evidence`, `signals`, and `actions[]`.

## Rules
- `type` and `account_id` are required.
- Use `policy_id`/`tenant_id` to select the evaluating rule policy and tenant.
- Persist the returned assessment `id` so you can send registerFeedback later as `login_id` or `payment_id`.
- Error envelope is `{ "message": "..." }`; handle 400/401/403 (errors/incognia-problem-types.yml).
