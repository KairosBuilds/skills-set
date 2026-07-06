# Database Architect Quality Checklist

## Pre-Delivery Validation

### Requirements Coverage
- [ ] All data requirements identified and addressed
- [ ] Workload patterns classified (OLTP/OLAP/HTAP)
- [ ] Performance requirements documented
- [ ] Data volume and growth projections included

### Data Modeling
- [ ] Conceptual model captures all entities and relationships
- [ ] Logical model includes all attributes and constraints
- [ ] Physical model includes all DDL statements
- [ ] ERD diagram provided and accurate

### Schema Design
- [ ] Tables have appropriate primary keys
- [ ] Foreign key relationships defined where needed
- [ ] Normalization level appropriate for workload
- [ ] Naming conventions followed

### Index Strategy
- [ ] Indexes designed for common query patterns
- [ ] No redundant or unused indexes
- [ ] Composite index column order optimized
- [ ] Index maintenance considered

### Query Optimization
- [ ] Common queries analyzed and optimized
- [ ] EXPLAIN plans reviewed for slow queries
- [ ] N+1 query patterns prevented
- [ ] Caching strategy defined

### Migration
- [ ] Migration scripts versioned and repeatable
- [ ] Zero-downtime migration approach designed
- [ ] Rollback procedures documented
- [ ] Data validation strategy defined

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Requirements Coverage | 15% | 100% |
| Data Modeling | 20% | >= 90% |
| Schema Design | 20% | 100% |
| Index Strategy | 15% | >= 90% |
| Query Optimization | 15% | >= 90% |
| Migration | 15% | 100% |
| **Overall** | **100%** | **>= 95%** |
