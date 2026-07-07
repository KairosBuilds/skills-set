# Database Architect Workflow

## Standard Design Flow

### Phase 1: Requirements Analysis
1. Understand data requirements and relationships
2. Identify workload patterns (OLTP, OLAP, mixed)
3. Define performance requirements (latency, throughput, concurrency)
4. Determine data volume and growth projections
5. Identify compliance and data governance requirements

### Phase 2: Database Selection
1. Evaluate database options (relational, document, key-value, graph, time-series, columnar)
2. Compare features against requirements
3. Consider operational complexity and team expertise
4. Make recommendation with ADR

### Phase 3: Data Modeling
1. Create conceptual data model (entity relationships)
2. Create logical data model (attributes, relationships, constraints)
3. Create physical data model (tables, columns, types, indexes)
4. Generate ERD diagram

### Phase 4: Schema Design
1. Write DDL statements
2. Design indexes for query patterns
3. Define constraints and validation rules
4. Plan partitioning and sharding strategy
5. Design migration scripts

### Phase 5: Query Optimization
1. Analyze common query patterns
2. Design indexes to support queries
3. Optimize slow queries using EXPLAIN
4. Design materialized views for reporting
5. Plan caching strategy

### Phase 6: Migration Planning
1. Design schema migration strategy (versioned, zero-downtime)
2. Plan data migration approach
3. Define rollback procedures
4. Create migration test plan

### Phase 7: Documentation
1. Compile data architecture document
2. Document schema with descriptions
3. Create query optimization guide
4. Document operations runbooks

## Output Template

```
1. Data Requirements Summary
2. Database Selection & Rationale
3. Data Model (Conceptual, Logical, Physical)
4. ERD Diagram
5. DDL Statements
6. Index Strategy
7. Query Optimization Guide
8. Partitioning Strategy
9. Migration Plan
10. Operations Guide
11. ADRs
```
