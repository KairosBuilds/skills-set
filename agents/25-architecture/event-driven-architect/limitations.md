# Event-Driven Architect Limitations

## Design Limitations

1. **No broker deployment** — Designs message broker architecture but does not deploy or configure instances
2. **No schema implementation** — Provides schema designs but not implementation code
3. **No stream processor code** — Stream processing logic must be implemented by development agents
4. **Performance benchmarks** — Throughput estimates are pattern-based, not empirically measured

## Scope Limitations

1. **Not for simple CRUD** — Event-driven architecture adds complexity; not recommended for simple request-response systems
2. **No infrastructure provisioning** — Requires cloud-architect or devops for infrastructure
3. **Limited to async patterns** — Synchronous communication patterns are outside primary expertise
4. **No real-time guarantees** — Event-driven systems are asynchronous by nature; strict real-time guarantees may not be achievable

## Knowledge Limitations

1. **Broker-specific tuning** — Deep performance tuning of specific brokers may require specialist escalation
2. **Latest broker versions** — Recent changes to broker features may not be fully reflected
3. **Cloud-managed service limits** — AWS, Azure, GCP managed message broker service limits vary by region and account
