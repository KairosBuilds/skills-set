# System Architect Examples

## Example 1: High-Throughput Data Pipeline

**Request:** "Design a system that processes 10M events per minute"

**Output:**
- Architecture: Kafka → Stream Processor (Flink) → Data Lake (S3/Parquet) → Analytics Engine (Presto)
- Scalability: Kafka partitioning by event type, auto-scaling stream processors, read replicas for analytics
- Reliability: Replication factor 3 for Kafka, checkpointing for Flink, S3 durability 99.999999999%
- Performance: Estimated throughput 200K events/second per partition with < 100ms processing latency
- Operations: Prometheus metrics, structured logging, distributed tracing with OpenTelemetry

## Example 2: Multi-Region Deployment

**Request:** "Design a globally distributed system with < 50ms p99 latency"

**Output:**
- Architecture: Active-active multi-region with global load balancer
- Data: Geo-partitioned databases with cross-region replication, local read replicas
- Consistency: Eventual consistency for reads, strong consistency for writes via Paxos-based reconciliation
- Failover: Automatic DNS failover, database promotion, traffic draining for degraded regions
- ADR: Documented trade-offs between consistency and latency across regions

## Example 3: System Reliability Review

**Request:** "Our system has 99.5% uptime, we need 99.99%. What needs to change?"

**Output:**
- Gap analysis: Single database, no redundancy for critical services, manual failover
- Recommendations: Active-passive database with auto-failover, redundant service instances, automated health checks
- Expected improvement: 99.5% → 99.99% with estimated cost increase of 40%
- Migration plan: Phased rollout over 3 months
