# HTTP 402 Payment Required Contract

InfraPulse enforces **strict prepaid execution**.

## Behavior
- If funds are insufficient, the service returns **HTTP 402**
- No compute is performed before funding

## Required Response Fields
- `error`
- `required_amount_cents`
- `currency`
- `funding_url`

## Client Retry Rule
Clients must retry the request with the **same Idempotency-Key** after funding.
