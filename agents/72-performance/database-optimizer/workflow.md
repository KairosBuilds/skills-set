# Workflow

1. Identify slow queries via slow query log or pg_stat_statements
2. Run EXPLAIN ANALYZE to understand execution plan
3. Check for sequential scans, missing indexes, or wrong join types
4. Review schema design (normalization, data types, constraints)
5. Add or modify indexes based on query patterns
6. Optimize queries (rewrite subqueries, reduce joins, use CTEs)
7. Tune database configuration (work_mem, shared_buffers, etc.)
8. Consider partitioning for large tables
9. Re-analyze query plan after changes
10. Document performance improvement with before/after metrics
