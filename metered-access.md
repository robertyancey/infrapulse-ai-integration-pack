# Metered Access (HTTP 402)

InfraPulse.ai uses HTTP 402 as a deterministic signaling mechanism for metered AI execution.

## Flow
1. Agent discovers service via beacon
2. Agent evaluates pricing and policy
3. Request is made
4. If insufficient credits → HTTP 402 returned
5. Upon payment or authorization → execution proceeds
6. Signed receipt is issued

## Purpose
This enables autonomous agents to reason about cost, authorization, and execution without human intervention, while remaining auditable and controllable.
