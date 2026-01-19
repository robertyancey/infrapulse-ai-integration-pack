# InfraPulse Services (Machine-Oriented)

All services are **prepaid-only**.
If insufficient funds exist, InfraPulse returns **HTTP 402 Payment Required**.

## Infrastructure Health Score
- Endpoint: `GET /v2/infra/health-score`
- Purpose: Numeric health signal for autonomous decision-making

## Infrastructure Verdict
- Endpoint: `GET /v2/infra/verdict`
- Purpose: Deterministic pass/fail gate for automation

## Failure Prediction
- Endpoint: `POST /predict/failure`
- Purpose: Predict probability of infrastructure failure

## Architecture Analysis
- Endpoint: `POST /v2/architecture/analyze`
- Purpose: Identify architectural risks and bottlenecks

## Smart Routing
- Endpoint: `POST /v1/smart-route`
- Purpose: Deterministic provider/model routing
- Requires header: `Idempotency-Key`
- Returns: signed execution receipt
