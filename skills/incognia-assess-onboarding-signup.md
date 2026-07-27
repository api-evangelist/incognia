---
name: Assess an onboarding signup for fraud
description: Get a real-time low/high/unknown risk verdict for a new-user signup using Incognia.
api: openapi/incognia-openapi-original.yml
operations: [createToken, registerSignup]
---

# Assess an onboarding signup for fraud

Use this to evaluate a new user during onboarding and decide whether to allow, review, or block.

## Auth (operation: createToken)
1. `POST https://api.incognia.com/api/v2/token` with your `client_id`/`client_secret` as HTTP Basic credentials and `Content-Type: application/x-www-form-urlencoded`.
2. Read `access_token` and `expires_in` from the JSON response. Send `Authorization: Bearer <access_token>` on every subsequent call. Refresh before `expires_in` seconds elapse (SDKs do this automatically).

## Assess the signup (operation: registerSignup)
1. `POST /v2/onboarding/signups` with either an `installation_id` (from the mobile SDK) or a `request_token` (from the web SDK).
2. Optionally include the user's address (`address_line`, `structured_address`, or `address_coordinates`) to score address quality and location behavior, plus `account_id`/`external_id` and a `policy_id`.
3. Read `risk_assessment` from the response: `low_risk`, `high_risk`, or `unknown_risk`. Use `reasons[]`, `evidence`, and `signals` to explain the verdict, and `actions[]` for recommended handling.

## Rules
- Never log or persist `client_secret`; treat access tokens as short-lived secrets.
- Errors return `{ "message": "..." }` with status 400 (bad params), 401 (bad token), or 403 (not permitted) — see errors/incognia-problem-types.yml.
- Later, close the loop by calling registerFeedback with the returned `id` as `signup_id`.
