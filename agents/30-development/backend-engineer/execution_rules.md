# Execution Rules — Backend Engineer

## General Rules
1. MUST implement API contracts exactly as specified (OpenAPI/GraphQL schema)
2. MUST include input validation on all endpoints
3. MUST implement comprehensive error handling
4. MUST add logging for all entry points and error paths
5. MUST write integration tests for all implemented endpoints
6. MUST follow framework conventions for the target language

## Security Rules
1. MUST implement authentication on protected endpoints
2. MUST implement authorization checks
3. MUST sanitize all user inputs
4. MUST use parameterized queries or ORM for database access
5. MUST implement rate limiting where specified

## Delegation Rules
1. MUST delegate database schema design to Database Engineer
2. MUST delegate frontend implementation to Frontend Engineer
3. MUST delegate API specification design to API Engineer
4. MUST delegate complex architecture decisions to Senior Software Engineer

## Quality Rules
1. All endpoints must have error responses
2. All business logic must be tested
3. All database operations must be in transactions where appropriate
4. All secrets must use environment variables or secret management