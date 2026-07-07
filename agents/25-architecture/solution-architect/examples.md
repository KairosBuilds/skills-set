# Solution Architect Examples

## Example 1: Full System Design

**Request:** "Design a scalable e-commerce platform"

**Output Summary:**
- Architecture: Event-driven microservices with modular monolith for core checkout
- Components: Product Service, Order Service, Payment Service, Notification Service, Inventory Service
- Tech Stack: Node.js/TypeScript, PostgreSQL, RabbitMQ, Redis, AWS ECS
- Diagram: Multi-service architecture with API Gateway, message broker, and data stores
- ADRs: ADR-001 (Microservices vs Monolith), ADR-002 (PostgreSQL vs DynamoDB), ADR-003 (RabbitMQ vs Kafka)
- Risk Assessment: Distributed transaction complexity, eventual consistency challenges

## Example 2: Technology Selection

**Request:** "Should we use AWS Lambda or traditional servers for our API?"

**Output:**
- Evaluation criteria: cost at scale, cold start tolerance, team expertise, operational overhead
- Lambda: pros (no server management, auto-scaling, pay-per-use), cons (cold starts, 15min timeout, execution environment limits)
- ECS Fargate: pros (more control, longer execution, consistent performance), cons (higher baseline cost, more ops overhead)
- Recommendation: Lambda for bursty/sporadic workloads, ECS for steady-state high-throughput APIs
- ADR documenting decision with cost projections at different traffic levels

## Example 3: Architecture Review

**Request:** "Review our current architecture for scalability issues"

**Output:**
- Identified bottlenecks: monolithic database, synchronous inter-service calls, no caching layer
- Recommendations: Introduce read replicas, add message queue for async operations, implement CDN for static assets
- Priority: Database bottleneck (critical), sync calls (high), caching (medium)
- Risk: Migration complexity estimated at 2-3 sprints
