# Quality Checklist

- [ ] Slow query log is enabled and monitored
- [ ] EXPLAIN ANALYZE is used before optimization
- [ ] Indexes match actual query patterns
- [ ] No sequential scans on large tables
- [ ] Connection pooling is configured
- [ ] Composite indexes are preferred over multiple single-column
- [ ] Over-indexing is avoided on write-heavy tables
- [ ] Large tables (> 100M rows) are partitioned
- [ ] Database configuration is tuned (work_mem, shared_buffers)
- [ ] Before/after query times documented
