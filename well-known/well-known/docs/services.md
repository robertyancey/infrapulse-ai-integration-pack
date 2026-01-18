# InfraPulse Services (Machine-Oriented)

## Paid Services (Prepaid Only)

### Infrastructure Health Score
- Endpoint: /v2/infra/health-score
- Purpose: Numeric health signal for agents

### Infrastructure Verdict
- Endpoint: /v2/infra/verdict
- Purpose: Deterministic pass/fail gate

### Failure Prediction
- Endpoint: /predict/failure
- Purpose: Outage probability forecast

### Architecture Analysis
- Endpoint: /v2/architecture/analyze
- Purpose: Risk and design analysis

### Smart Routing
- Endpoint: /v1/smart-route
- Purpose: Provider/model routing with receipts
- Requires: Idempotency-Key
