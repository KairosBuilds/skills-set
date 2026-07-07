# Event-Driven Architect Workflow

## Standard Design Flow

### Phase 1: Event Discovery
1. Identify business events and domain events
2. Map event flows across the system
3. Identify event producers and consumers
4. Prioritize events by business criticality

### Phase 2: Broker Selection
1. Evaluate requirements: throughput, latency, retention, routing, durability
2. Compare broker options against requirements
3. Select primary and fallback brokers
4. Document selection rationale in ADR

### Phase 3: Event Schema Design
1. Define event schemas with clear naming conventions
2. Choose schema format (Avro, Protobuf, JSON Schema)
3. Configure schema registry with compatibility rules
4. Version events for evolution

### Phase 4: Topology Design
1. Design topic/queue structure
2. Define partitioning strategy
3. Design routing and filtering
4. Plan consumer group structure

### Phase 5: Reliability Design
1. Design delivery semantics (at-least-once, exactly-once)
2. Implement dead letter queues
3. Design retry and backoff strategies
4. Plan monitoring and alerting

### Phase 6: Stream Processing (if needed)
1. Identify stream processing requirements
2. Choose stream processor (Kafka Streams, Flink, Spark Streaming)
3. Design processing topology
4. Plan state management

### Phase 7: Documentation
1. Create event catalog
2. Document topology diagrams
3. Write producer/consumer contracts
4. Create operations runbooks

## Output Template

```
1. Event Catalog
2. Broker Selection & Rationale
3. Event Schema Definitions
4. Topology Diagram
5. Producer/Consumer Contracts
6. Delivery Semantics Design
7. Dead Letter & Retry Strategy
8. Stream Processing Design
9. Monitoring & Alerting
10. Operations Runbook
11. ADRs
```
