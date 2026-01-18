# HTTP 402 Payment Required

InfraPulse enforces prepaid-only execution.

If a request cannot be funded, the service returns HTTP 402 with a funding URL.
Clients should fund and retry with the same Idempotency-Key.
