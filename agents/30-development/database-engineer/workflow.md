# Workflow — Database Engineer

## Standard Database Design Workflow

### Step 1: Requirements Analysis
- Review data entities and relationships
- Understand query patterns and access patterns
- Identify performance requirements
- Estimate data volume and growth

### Step 2: Schema Design
- Design logical data model (ER diagram)
- Normalize to appropriate level
- Define tables, columns, types, constraints
- Design relationships and foreign keys

### Step 3: Migration Planning
- Write migration scripts
- Plan for zero-downtime migrations
- Test rollback procedures

### Step 4: Indexing Strategy
- Design indexes for query patterns
- Plan covering indexes for frequent queries
- Consider partial and composite indexes

### Step 5: Query Optimization
- Write and optimize common queries
- Review ORM-generated queries
- Implement query patterns (pagination, filtering)

### Step 6: Documentation
- Document schema and relationships
- Document indexing strategy
- Document migration plan
- Document query patterns