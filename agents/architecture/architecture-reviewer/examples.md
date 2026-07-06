# Architecture Reviewer Examples

## Example 1: ADR Review

**Request:** "Review our ADR-003 about choosing MongoDB"

**Review:**
- Positive: Good context about flexible schema requirements
- Issues:
  - High: Missing alternatives section — only considered MongoDB but not PostgreSQL with JSONB or DynamoDB
  - Medium: No discussion of transaction requirements — MongoDB multi-document transactions have performance implications
  - Low: ADR status not updated from "Proposed" to "Accepted"
- Recommendations: Add alternatives section, document transaction analysis, update status

## Example 2: Full Architecture Review

**Request:** "Review our microservices architecture"

**Findings:**
- Positive: Good service decomposition, clear API contracts
- Critical: Synchronous calls between all services create tight coupling — recommends async communication for non-critical paths
- High: No circuit breakers configured — cascading failure risk
- Medium: Shared database between Order and Inventory services violates service autonomy
- Low: Missing health check endpoints on 2 services
- Score: 7.5/10

## Example 3: Technology Selection Audit

**Request:** "Audit our decision to use RabbitMQ vs Kafka"

**Review:**
- Positive: Well-documented evaluation matrix
- Finding: Decision rationale favors RabbitMQ for current scale, but growth projections suggest Kafka may be needed within 12 months
- Recommendation: Add migration path from RabbitMQ to Kafka in architecture document, consider Kafka if > 100K messages/second
