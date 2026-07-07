# GraphQL Architect Execution Rules

## Schema Design Rules

1. **Schema-first** — Always design the schema (SDL) before implementing resolvers
2. **Clear naming** — Use PascalCase for types, camelCase for fields; descriptive names over abbreviations
3. **Nullability** — Default to non-null where the data is guaranteed; use null for optional fields
4. **List types** — Use paginated connections for large lists, not raw lists
5. **Input types** — Use dedicated input types for mutations, never reuse field arguments

## Resolver Rules

1. **DataLoader for batching** — Always use DataLoader to batch and cache database queries within a request
2. **N+1 prevention** — Profile for N+1 queries; ensure DataLoader covers all relation lookups
3. **Resolver simplicity** — Resolvers should be thin; business logic belongs in service layer
4. **Error handling** — Use a union or interface pattern for mutation results to include user-facing errors
5. **Authorization** — Use declarative directives for auth checks; never embed auth logic in resolvers

## Federation Rules

1. **Single responsibility** — Each subgraph owns a specific domain; avoid overlapping entity definitions
2. **Entity keys** — Define @key directives carefully; prefer compound keys over single-field keys
3. **Reference resolvers** — All referenced entities must have __resolveReference resolvers
4. **Subgraph isolation** — Subgraphs should not call other subgraphs directly; use the gateway
5. **Versioning strategy** — Use graph composition for evolution; avoid breaking changes

## Performance Rules

1. **Complexity analysis** — Implement query complexity scoring to prevent expensive queries
2. **Depth limiting** — Limit maximum query depth (recommended: max 7-8 levels)
3. **Persisted queries** — Use persisted queries for production to prevent arbitrary queries
4. **Subscription throttling** — Implement rate limiting for subscriptions
5. **CDN caching** — Use CDN caching for public GET queries
