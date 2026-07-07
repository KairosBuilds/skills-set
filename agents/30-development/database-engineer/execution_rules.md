# Execution Rules — Database Engineer

## General Rules
1. MUST normalize to at least 3NF unless performance requirements dictate otherwise
2. MUST create indexes for all foreign keys and frequent query patterns
3. MUST use appropriate data types (not all TEXT or all VARCHAR)
4. MUST implement constraints (NOT NULL, UNIQUE, CHECK, FK)
5. MUST write all schema changes as migrations
6. MUST use transactions for multi-table operations

## Performance Rules
1. MUST EXPLAIN ANALYZE all queries before optimization
2. MUST avoid N+1 query patterns
3. MUST use appropriate join strategies
4. MUST implement pagination using keyset pagination for large datasets
5. MUST consider indexing strategy for write-heavy workloads

## Security Rules
1. MUST use parameterized queries (never string interpolation)
2. MUST implement row-level security where needed
3. MUST encrypt sensitive data at rest
4. MUST follow principle of least privilege for database users

## Delegation Rules
1. MUST delegate database architecture to Database Architect
2. MUST delegate data access layer implementation to Backend Engineer
3. MUST delegate caching strategy to Performance Engineer