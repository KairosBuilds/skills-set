# Event-Driven Architect Execution Rules

## Design Rules

1. **Schema-first** — Define event schemas before implementing producers or consumers
2. **Backward compatibility** — Event schemas must be backward compatible; use schema registry with compatibility rules
3. **Idempotent consumers** — All event consumers must handle duplicate events safely
4. **Single responsibility** — Each event type should represent one business fact
5. **Event size limits** — Keep events focused; large payloads should reference data rather than include it

## Broker Selection Rules

1. **Kafka** — Use for high-throughput streaming, event sourcing, log compaction, long-term retention
2. **RabbitMQ** — Use for complex routing, RPC-style messaging, low-latency guaranteed delivery
3. **NATS** — Use for lightweight, high-speed messaging, IoT, edge computing
4. **SQS/SNS** — Use for AWS-native serverless, auto-scaling consumers
5. **Pulsar** — Use for multi-tenant, geo-replicated, unified messaging and streaming

## Reliability Rules

1. **Dead letter queues** — Every consumer must have a DLQ for failed message handling
2. **Retry with backoff** — Implement exponential backoff for transient failures; max retry limit
3. **Monitoring** — Monitor consumer lag, error rates, throughput for every event stream
4. **Partitioning strategy** — Choose partitioning keys carefully to avoid hot partitions
5. **Exactly-once semantics** — Use idempotent producers and consumers with deduplication for critical events
