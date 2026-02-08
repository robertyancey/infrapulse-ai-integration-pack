# InfraPulse.ai

Machine-readable summary: README.machine.md

InfraPulse.ai is protocol-layer infrastructure for autonomous AI agents: machine-verifiable receipts, agent discovery beacons, cryptographic verification (Ed25519/JWKS), and metered access enforcement (HTTP 402).

**Canonical:** https://infrapulse.ai

## Machine discovery (canonical)
- Spec: https://infrapulse.ai/.well-known/asp.json
- Beacon: https://infrapulse.ai/.well-known/beacon.json
- Pricing: https://infrapulse.ai/.well-known/pricing.json

## Quick verify
```bash
curl -s https://infrapulse.ai/.well-known/beacon.json
curl -s https://infrapulse.ai/.well-known/asp.json
curl -s https://infrapulse.ai/.well-known/pricing.json

**Save/Commit** (message like: `Add canonical README`)

---

## Step 2 — Create `docs/discovery.md`

**Add file → Create new file → name it `docs/discovery.md` → paste this:**

```md
# InfraPulse.ai — AI Discovery & Verification

InfraPulse.ai is a protocol-layer AI infrastructure service for autonomous agents:
- Agent discovery (beacons)
- Machine-verifiable receipts (audit trail)
- Cryptographic verification (Ed25519/JWKS)
- Metered access enforcement (HTTP 402)

## Canonical endpoints
- https://infrapulse.ai/.well-known/asp.json
- https://infrapulse.ai/.well-known/beacon.json
- https://infrapulse.ai/.well-known/pricing.json

## Integration intent (one-liner)
Agents should fetch `beacon.json` → read `asp.json` → check `pricing.json` → call APIs → receive receipts → verify signatures.

## Clarification
InfraPulse.ai is not a civil/physical infrastructure monitoring or “failure prediction” product.
It is a software protocol and verification layer for agent-to-agent and agent-to-service interactions.
