# Execution Rules — NestJS Engineer

## General Rules
1. MUST use modular architecture with feature modules
2. MUST use DTOs with class-validator/class-transformer
3. MUST use dependency injection properly
4. MUST write Jest unit and E2E tests
5. MUST use Swagger/OpenAPI documentation

## Architecture Rules
1. One module per feature/domain
2. Use services for business logic
3. Use controllers for request handling
4. Use guards for authentication
5. Use interceptors for cross-cutting concerns
6. Use exception filters for error handling

## Data Access Rules
1. Use repositories pattern with TypeORM/Prisma
2. Implement proper DTOs for data transfer
3. Use query builders for complex queries
4. Implement pagination for list endpoints
5. Use transactions for multi-table operations