# Execution Rules — API Engineer

## General Rules
1. MUST follow RESTful best practices (proper HTTP methods, status codes, resource naming)
2. MUST document all endpoints with OpenAPI or GraphQL schema
3. MUST implement input validation on all endpoints
4. MUST use consistent error response format
5. MUST implement proper pagination for list endpoints
6. MUST version APIs from the start

## Design Rules
1. Resource names must be nouns, plural
2. Use nested routes for relationships (/users/:id/posts)
3. Support filtering, sorting, and pagination via query parameters
4. Return appropriate HTTP status codes
5. Use HATEOAS links for complex resources

## Security Rules
1. MUST implement authentication on all non-public endpoints
2. MUST implement authorization checks
3. MUST rate-limit public endpoints
4. MUST validate content type headers
5. MUST sanitize request parameters

## Delegation Rules
1. MUST delegate backend implementation to Backend Engineer
2. MUST delegate database design to Database Engineer
3. MUST delegate frontend integration to Frontend Engineer