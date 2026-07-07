# API Designer Execution Rules

## REST Design Rules

1. **Resource-oriented** — APIs should be organized around resources (nouns), not actions (verbs)
2. **Proper HTTP methods** — GET for retrieval, POST for creation, PUT for full update, PATCH for partial update, DELETE for removal
3. **Standard status codes** — Use appropriate HTTP status codes (200, 201, 204, 400, 401, 403, 404, 409, 422, 500)
4. **Consistent naming** — Use plural nouns for collections, kebab-case for URL paths, camelCase for JSON fields
5. **Pagination** — All list endpoints must support pagination (cursor-based preferred for consistency)
6. **Error format** — Consistent error response structure with code, message, and details

## GraphQL Design Rules

1. **Schema-first** — Define SDL before implementing resolvers
2. **Single responsibility** — Each type and field should have a clear purpose
3. **N+1 prevention** — Use DataLoader for batching and caching
4. **Proper mutations** — Mutations return the modified object; include user-facing errors in the response
5. **Subscription considerations** — Use subscriptions for real-time events, not query substitutes
6. **Cost analysis** — Implement query complexity analysis to prevent abusive queries

## gRPC Design Rules

1. **Proto-first** — Define .proto files before implementing services
2. **Streaming patterns** — Choose appropriate streaming: unary, server-streaming, client-streaming, bidirectional
3. **Error handling** — Use standard gRPC status codes and error details
4. **Versioning** — Use package-level versioning in proto packages
5. **Backward compatibility** — Follow Protobuf best practices for field evolution
