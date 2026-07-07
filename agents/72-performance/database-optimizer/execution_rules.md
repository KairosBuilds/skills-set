# Execution Rules

1. Always analyze query plans before optimizing (EXPLAIN ANALYZE)
2. Never add indexes without understanding query patterns
3. One index per query optimization — measure before/after
4. Prefer composite indexes over multiple single-column indexes
5. Avoid over-indexing on write-heavy tables
6. Use connection pooling to reduce connection overhead
7. Monitor slow query logs continuously
8. Partition large tables (> 100M rows) by date or key
9. Normalize for consistency, denormalize for read performance
10. Never run untested schema changes in production
