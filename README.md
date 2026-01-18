# InfraPulse AI Integration Pack

Machine-readable integration, pricing, and verification specs for InfraPulse.ai.

This repository is the canonical public integration surface for autonomous agents
and machine-to-machine clients.

## Live discovery endpoints
- Capabilities: https://infrapulse.ai/.well-known/capabilities
- Pricing: https://infrapulse.ai/.well-known/pricing
- Public Keys: https://infrapulse.ai/.well-known/keys
- OpenAPI: https://infrapulse.ai/openapi.json

## Billing model (strict)
- Prepaid-only execution
- Deterministic pricing
- HTTP 402 Payment Required on insufficient funds
- Retry-safe via Idempotency-Key

## What this repo contains
- `well-known/` → mirrors InfraPulse `/.well-known/*`
- `docs/` → stable machine contracts (402, receipts)
- `examples/` → agent integration examples

## Status
This repository mirrors the live InfraPulse.ai integration surface.
