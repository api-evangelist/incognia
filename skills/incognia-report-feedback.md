---
name: Report a feedback event to tune the model
description: Send labeled outcomes (fraud, chargeback, accepted/declined) back to Incognia to improve future assessments.
api: openapi/incognia-openapi-original.yml
operations: [createToken, registerFeedback]
---

# Report a feedback event to tune the model

Close the loop by telling Incognia what actually happened after an assessment.

## Auth (operation: createToken)
Exchange `client_id`/`client_secret` (HTTP Basic) at `POST /v2/token` for a bearer token; send `Authorization: Bearer <access_token>`.

## Send feedback (operation: registerFeedback)
1. `POST /v2/feedbacks` with an `event` from the supported set, for example: `account_takeover`, `identity_fraud`, `chargeback`, `promotion_abuse`, `signup_accepted`, `signup_declined`, `login_accepted`, `login_declined`, `payment_accepted`, `payment_declined`, `verified`, `account_allowed`.
2. Identify the subject with the strongest identifier(s) you have: `signup_id`, `login_id`, `payment_id` (the assessment `id` you stored earlier), or `account_id` / `external_id` / `installation_id` / `request_token`.
3. Set `occurred_at` (and optionally `expires_at`) to timestamp the event.

## Rules
- `event` is required; identifiers should reference a prior assessment when possible so feedback is attributed correctly.
- Feedback is fire-and-forget (a 200 with no body on success); handle 400/401 error envelopes `{ "message": "..." }`.
- Reporting confirmed fraud and confirmed-good outcomes both improve model accuracy — send both.
