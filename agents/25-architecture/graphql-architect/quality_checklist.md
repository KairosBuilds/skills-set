# GraphQL Architect Quality Checklist

## Pre-Delivery Validation

### Schema Design
- [ ] Types, interfaces, and unions clearly defined
- [ ] Naming conventions followed (PascalCase types, camelCase fields)
- [ ] Nullability appropriately configured
- [ ] Input types used for mutations
- [ ] Pagination implemented for list fields
- [ ] Deprecation directives used where appropriate

### Resolver Architecture
- [ ] DataLoader implemented for all relation lookups
- [ ] N+1 query patterns prevented
- [ ] Resolvers are thin (logic in service layer)
- [ ] Error handling pattern defined (union/interface)
- [ ] Authorization directives used

### Federation (if applicable)
- [ ] Subgraph boundaries align with service boundaries
- [ ] @key directives correctly defined
- [ ] __resolveReference implemented for all entities
- [ ] Subgraphs are independent (no cross-subgraph calls)
- [ ] Supergraph composition works

### Performance
- [ ] Query complexity analysis configured
- [ ] Depth limiting set (max 7-8)
- [ ] DataLoader caching strategy defined
- [ ] Persisted queries considered for production
- [ ] Subscription throttling considered

### Security
- [ ] Authentication directives defined
- [ ] Authorization roles/permissions mapped
- [ ] Rate limiting strategy defined
- [ ] Query whitelisting considered

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Schema Design | 25% | 100% |
| Resolver Architecture | 20% | >= 90% |
| Federation | 20% | >= 90% |
| Performance | 20% | >= 90% |
| Security | 15% | 100% |
| **Overall** | **100%** | **>= 95%** |
