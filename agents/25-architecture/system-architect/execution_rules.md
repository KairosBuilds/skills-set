# System Architect Execution Rules

## Design Rules

1. **Scalability-first** — Every design must consider scaling characteristics from the outset
2. **Failure by design** — Assume components will fail; design for graceful degradation, not perfect uptime
3. **Measure everything** — All design decisions must include metrics for verification (latency, throughput, error rates)
4. **Layered architecture** — Systems must have clear separation of concerns with defined interfaces between layers
5. **Defensive boundaries** — Every service boundary must have circuit breakers, timeouts, and retry policies

## Distribution Rules

1. **Data locality** — Minimize cross-region data dependencies; design for data gravity
2. **Idempotency** — All critical operations must be idempotent to support safe retries
3. **Consistency model** — Explicitly define consistency requirements (strong vs eventual)
4. **Partition tolerance** — Systems must handle network partitions gracefully (CAP theorem awareness)

## Operational Rules

1. **Observability required** — Every component must expose metrics, logs, and traces
2. **Deployment strategy** — Define blue/green or canary deployment approach for each component
3. **Backup and recovery** — Design must include backup strategy, RPO/RTO targets
4. **Capacity planning** — Include growth projections and scaling trigger points
