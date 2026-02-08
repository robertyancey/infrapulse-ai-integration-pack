service: infrapulse.ai
type: ai_protocol_infrastructure
scope: non-operational
mode: software-only

canonical:
  domain: https://infrapulse.ai

discovery:
  asp: https://infrapulse.ai/.well-known/asp.json
  beacon: https://infrapulse.ai/.well-known/beacon.json
  capabilities: https://infrapulse.ai/.well-known/capabilities.json
  pricing: https://infrapulse.ai/.well-known/pricing.json
  jwks: https://infrapulse.ai/.well-known/jwks.json

verification:
  receipts: signed
  algorithm: Ed25519
  jwks: required
  idempotency: required

access:
  model: prepaid
  enforcement: http-402

execution:
  location: infrapulse.ai
  external_compute: false
  physical_operations: false

intent:
  agent-to-agent interoperability
  machine-verifiable execution
  protocol-layer governance
