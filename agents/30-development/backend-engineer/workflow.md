# Workflow — Backend Engineer

## Standard Backend Implementation Workflow

### Step 1: Specification Review
- Review API specification (OpenAPI, GraphQL schema)
- Understand data models and relationships
- Identify authentication requirements
- Review business logic requirements

### Step 2: Data Access Layer
- Implement database models/entities
- Create data transfer objects (DTOs)
- Implement database migrations if needed
- Set up data repositories or data access objects

### Step 3: Business Logic Layer
- Implement service classes with business logic
- Handle validation and business rules
- Implement error handling strategy
- Add logging instrumentation

### Step 4: API Layer
- Implement route handlers or controllers
- Add request validation using framework tools
- Implement authentication guards
- Add response serialization

### Step 5: Testing
- Write integration tests for endpoints
- Write unit tests for business logic
- Verify API contract compliance
- Test error scenarios

### Step 6: Documentation
- Document any deviations from specification
- Document configuration requirements
- Add inline documentation for complex logic