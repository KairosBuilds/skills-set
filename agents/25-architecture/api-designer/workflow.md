# API Designer Workflow

## Standard Design Flow

### Phase 1: Requirements Gathering
1. Understand API consumers and use cases
2. Identify resources and operations needed
3. Determine protocol requirements (REST, GraphQL, gRPC)
4. Define performance and security requirements

### Phase 2: API Design
1. Model resources and relationships
2. Design endpoints/mutations/queries/services
3. Define request/response schemas
4. Design error handling patterns
5. Plan authentication and authorization

### Phase 3: Specification
1. Write OpenAPI specification / GraphQL SDL / Protobuf definitions
2. Include examples for all endpoints
3. Define security schemes
4. Document edge cases and error responses

### Phase 4: Review
1. Validate specification against design rules
2. Check consistency and completeness
3. Review with stakeholders
4. Iterate based on feedback

### Phase 5: Documentation
1. Generate API reference documentation
2. Create getting-started guide
3. Provide SDK usage examples
4. Document breaking changes and migration

### Phase 6: Governance
1. Define API versioning strategy
2. Establish API change management process
3. Document deprecation policy
4. Plan API monitoring and metrics

## Output Template (REST)

```
1. API Overview
2. Authentication & Authorization
3. Resource Model
4. Endpoint Reference
5. Request/Response Schemas
6. Error Handling
7. Pagination & Filtering
8. Rate Limiting
9. Versioning Strategy
10. OpenAPI Specification (YAML/JSON)
11. Usage Examples
```
