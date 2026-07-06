# Database Architect Execution Rules

## Design Rules

1. **Normalize until it hurts, denormalize until it works** — Start normalized and denormalize for performance only with measured justification
2. **Primary keys are mandatory** — Every table must have a primary key; prefer UUIDs for distributed systems, auto-increment for simple cases
3. **Foreign key integrity** — Use foreign keys for referential integrity; document exceptions explicitly
4. **Index with purpose** — Every index must have a clear use case; avoid over-indexing
5. **Naming conventions** — Consistent naming: snake_case for tables and columns, singular for table names, plural for join tables

## Query Rules

1. **EXPLAIN before optimization** — Always analyze query plans before making optimization decisions
2. **Index matching** — Indexes must match query patterns (composite index column order matters)
3. **Avoid N+1** — Use JOINs, eager loading, or batch queries to prevent N+1 query problems
4. **Limit result sets** — Always use LIMIT for queries that don't need full result sets
5. **Connection pooling** — Use connection pooling for production applications

## Selection Rules

1. **ACID for transactions** — Use relational databases when ACID compliance is required
2. **NoSQL for scale** — Use NoSQL for horizontal scalability, flexible schemas, or specific data models (document, graph, time-series)
3. **Workload matching** — Choose database type based on workload (OLTP, OLAP, HTAP)
4. **Managed vs self-hosted** — Prefer managed databases for operational simplicity unless compliance requires self-hosting
5. **Consistency requirements** — Choose based on consistency needs (strong vs eventual)
