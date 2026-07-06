# Microservices Architect Workflow

## Standard Design Flow

### Phase 1: Domain Analysis
1. Understand business domain and capabilities
2. Identify bounded contexts using DDD
3. Map domain events and aggregates
4. Document ubiquitous language

### Phase 2: Service Identification
1. Decompose bounded contexts into candidate services
2. Define service responsibilities and APIs
3. Identify service dependencies (avoid circular)
4. Validate service boundaries with business stakeholders

### Phase 3: Communication Design
1. Identify communication patterns per interaction
2. Design events and message schemas
3. Define synchronous API contracts (REST/gRPC)
4. Document communication matrix

### Phase 4: Data Architecture
1. Assign data ownership per service
2. Design data models per service
3. Plan data sharing and replication
4. Design saga flows for multi-service operations

### Phase 5: Operational Design
1. Design service discovery mechanism
2. Plan API gateway / BFF strategy
3. Design deployment topology
4. Plan monitoring and observability per service

### Phase 6: Migration Planning
1. Identify decomposition sequence
2. Plan strangler fig or branch-by-abstraction approach
3. Define success metrics for each migration phase
4. Create rollout timeline

## Output Template

```
1. Domain Analysis (DDD)
2. Service Catalog
3. Service Boundaries Diagram
4. Communication Matrix
5. API Contracts
6. Data Ownership Map
7. Saga Flows
8. Deployment Topology
9. Migration Plan
10. ADRs
```
