# GraphQL Architect Workflow

## Standard Design Flow

### Phase 1: Requirements Analysis
1. Understand client data requirements and usage patterns
2. Identify entities, relationships, and operations
3. Determine auth requirements
4. Define performance requirements

### Phase 2: Schema Design
1. Define types, interfaces, and unions
2. Design query root fields
3. Design mutation root fields
4. Design subscription root fields
5. Define input types and enums
6. Write SDL

### Phase 3: Resolver Architecture
1. Design resolver structure per type
2. Implement DataLoader patterns
3. Design error handling strategy
4. Plan authorization directives

### Phase 4: Federation (if applicable)
1. Identify subgraph boundaries
2. Define entity keys and references
3. Design supergraph composition
4. Plan subgraph deployment

### Phase 5: Performance & Security
1. Set query complexity limits
2. Configure depth limiting
3. Implement persisted queries
4. Design caching strategy
5. Plan rate limiting

### Phase 6: Documentation
1. Generate schema documentation
2. Create resolver reference
3. Document query examples
4. Provide client usage guide

## Output Template

```
1. Schema Overview
2. SDL Definition
3. Type Catalog
4. Resolver Architecture
5. DataLoader Design
6. Error Handling Strategy
7. Federation Design (if applicable)
8. Performance Optimization
9. Security Measures
10. Client Usage Guide
11. ADRs
```
