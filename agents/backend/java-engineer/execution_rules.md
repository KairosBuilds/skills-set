# Execution Rules — Java Engineer

## General Rules
1. MUST use Java 21+ features (records, sealed classes, pattern matching)
2. MUST use proper dependency injection (Spring DI)
3. MUST write JUnit 5 tests with Mockito
4. MUST use SLF4J for logging
5. MUST handle exceptions properly (checked vs unchecked)

## Spring Boot Rules
1. Use constructor injection (not field injection)
2. Implement proper layered architecture (controller, service, repository)
3. Use DTOs for API requests/responses
4. Implement proper exception handling with @ControllerAdvice
5. Use @Valid for request validation

## JPA Rules
1. Use @EntityGraph for N+1 query prevention
2. Use projections for read-only queries
3. Implement proper cascade types
4. Use pagination for list endpoints
5. Configure proper fetch types