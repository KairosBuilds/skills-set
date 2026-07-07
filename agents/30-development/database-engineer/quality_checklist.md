# Quality Checklist — Database Engineer

## Schema Quality
- [ ] Tables are normalized to at least 3NF
- [ ] Appropriate data types used
- [ ] Constraints defined (PK, FK, UNIQUE, CHECK, NOT NULL)
- [ ] Foreign keys have indexes
- [ ] Naming conventions consistent

## Migration Quality
- [ ] Migrations are reversible
- [ ] Rollback scripts prepared
- [ ] Zero-downtime approach documented
- [ ] Data integrity checks in place

## Performance Quality
- [ ] Frequent queries have indexes
- [ ] EXPLAIN ANALYZE reviewed for critical queries
- [ ] N+1 query patterns eliminated
- [ ] Pagination uses keyset pagination for large sets
- [ ] Connection pooling configured

## Security
- [ ] Parameterized queries used
- [ ] Sensitive data encrypted
- [ ] Least privilege principle applied
- [ ] SQL injection prevented