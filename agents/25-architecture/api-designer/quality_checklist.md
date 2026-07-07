# API Designer Quality Checklist

## Pre-Delivery Validation

### Design Quality
- [ ] Resources modeled as nouns (REST) or types (GraphQL)
- [ ] HTTP methods used correctly (REST)
- [ ] Consistent naming conventions throughout
- [ ] Error responses have consistent format
- [ ] Pagination designed for list endpoints

### Specification
- [ ] OpenAPI/SDL/Protobuf specification complete and valid
- [ ] All endpoints/mutations/services documented
- [ ] Request/response schemas defined
- [ ] Examples provided for all operations
- [ ] Security schemes defined (auth, permissions)

### Versioning & Evolution
- [ ] Versioning strategy defined
- [ ] Deprecation policy documented
- [ ] Breaking change policy stated
- [ ] Backward compatibility considered

### Security
- [ ] Authentication mechanism defined
- [ ] Authorization/permissions documented
- [ ] Rate limiting strategy designed
- [ ] Input validation approach described

### Documentation
- [ ] API reference documentation generated
- [ ] Getting-started guide included
- [ ] Usage examples provided
- [ ] Error code reference documented

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Design Quality | 25% | >= 90% |
| Specification | 25% | 100% |
| Versioning | 15% | 100% |
| Security | 20% | 100% |
| Documentation | 15% | >= 90% |
| **Overall** | **100%** | **>= 95%** |
