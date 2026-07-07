# Microservices Architect Execution Rules

## Decomposition Rules

1. **Domain-driven** — Service boundaries must follow business domain boundaries (bounded contexts), not technical layers
2. **Database per service** — Each service must own its data store; shared databases are an anti-pattern
3. **Service autonomy** — Services must be independently deployable, scalable, and testable
4. **Size guidelines** — Services should be sized by business capability, not technical convenience
5. **Migration incremental** — Decompose incrementally; big-bang rewrites are high-risk

## Communication Rules

1. **Async-first** — Prefer asynchronous communication (events, messaging) for cross-service interaction
2. **Sync only when needed** — Synchronous calls are acceptable for queries and real-time needs but must have timeouts and circuit breakers
3. **Idempotent operations** — All critical operations must be idempotent for safe retries
4. **Bulkhead pattern** — Isolate service failures to prevent cascading failures
5. **Retry with backoff** — Implement exponential backoff for retries, never retry indefinitely

## Data Rules

1. **Data ownership** — Each service has exclusive ownership of its data; access only via the service API
2. **Eventual consistency** — Accept eventual consistency across services where strong consistency isn't required
3. **Saga pattern** — Use sagas for distributed transactions; never use distributed transactions (2PC)
4. **CQRS consideration** — Consider CQRS for services with different read/write patterns
5. **Transactional outbox** — Use outbox pattern for reliable event publishing
