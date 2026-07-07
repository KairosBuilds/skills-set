# Event-Driven Architect Examples

## Example 1: E-Commerce Event Architecture

**Request:** "Design event architecture for our e-commerce platform"

**Output:**
- Events identified: OrderPlaced, PaymentProcessed, InventoryReserved, OrderConfirmed, ShipmentCreated, OrderDelivered
- Broker: Kafka (high throughput, log compaction for event sourcing)
- Schema: Avro with schema registry, backward compatibility
- Topology: 6 topics, partitioned by order_id, 3 partitions each
- Consumer groups: OrderService, PaymentService, InventoryService, NotificationService, AnalyticsService
- Reliability: At-least-once delivery, DLQ per consumer, retry 3x with exponential backoff
- Monitoring: Consumer lag alerts at 1000 messages, error rate alerts at 1%

## Example 2: Broker Selection

**Request:** "Which message broker should we use for IoT device telemetry?"

**Analysis:**
- Requirements: 100K messages/second per device group, variable payload sizes, need for long-term retention, multi-tenant
- Candidates: Kafka, RabbitMQ, NATS, Pulsar
- Recommendation: Apache Pulsar — native multi-tenancy, tiered storage for long retention, low latency
- ADR documenting trade-offs: Kafka (better ecosystem) vs Pulsar (better multi-tenancy and geo-replication)

## Example 3: Event Sourcing Design

**Request:** "Design event sourcing for our financial transaction system"

**Output:**
- Events: AccountCreated, FundsDeposited, FundsWithdrawn, TransferInitiated, TransferCompleted
- Event Store: Kafka with log compaction (compact by account_id for state reconstruction)
- Snapshots: Periodic state snapshots every 1000 events per account
- Projections: Current balance, transaction history, daily summaries
- CQRS: Separate read models for queries, write models for commands
- Compliance: Immutable event log for audit trail, 7-year retention
