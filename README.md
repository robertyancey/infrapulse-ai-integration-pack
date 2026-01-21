# InfraPulse AI Integration Pack


## Machine Discovery

InfraPulse is designed for autonomous agent usage.

Agent Manifest:
https://infrapulse.ai/.well-known/agent.json

Capabilities:
https://infrapulse.ai/.well-known/capabilities

Pricing:
https://infrapulse.ai/.well-known/pricing

OpenAPI:
https://infrapulse.ai/openapi.json

Health:
https://infrapulse.ai/api/v1/health

Billing Model:
Prepaid only, escrow supported, deterministic settlement

Package Name:
infrapulse

Description:
Python client for InfraPulse — deterministic, prepaid infrastructure services for autonomous agents.

Service URL:
https://infrapulse.ai

OpenAPI:
https://infrapulse.ai/openapi.json

Billing:
Prepaid, escrow-aware, no credit risk

Audience:
Autonomous agents, orchestration systems, AI platforms

Service Name:
InfraPulse

Category:
Infrastructure / Billing / Compute

Description:
Deterministic, prepaid infrastructure services for autonomous agents with escrow-aware settlement and real-time usage metering.

Base URL:
https://infrapulse.ai

Agent Manifest:
https://infrapulse.ai/.well-known/agent.json

Capabilities:
https://infrapulse.ai/.well-known/capabilities

Pricing:
https://infrapulse.ai/.well-known/pricing

OpenAPI:
https://infrapulse.ai/openapi.json

Authentication:
API key (Authorization: Bearer)

Billing Model:
Prepaid only (no credit fronting)

Escrow:
Supported

Human UI Required:
No

Health Check:
https://infrapulse.ai/api/v1/health

Contact:
robertspenceryancey@gmail.com



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
