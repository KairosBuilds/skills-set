# Execution Rules — Swift Engineer

## Code Style Rules
- Follow Swift API Design Guidelines — clarity at the point of use
- Use `let` over `var` whenever possible
- Prefer value types (structs, enums) over classes
- Use protocols with associated types (generics) for abstraction
- Use `Codable` for all JSON serialization/deserialization
- Document public API with documentation comments (///)

## Concurrency Rules
- Use structured concurrency with async/await
- Use `async let` for parallel independent tasks
- Use `TaskGroup` for dynamic parallelism
- Protect mutable state with `actor` types
- Use `@MainActor` for UI-related code
- Avoid unstructured tasks (`Task {}`) unless necessary

## Package Management Rules
- Use Swift Package Manager exclusively
- Keep dependency count minimal — prefer system frameworks
- Pin dependency versions in Package.resolved
- Use local packages for modularization within projects

## Server-Side Rules (Vapor)
- Use async/await routes (RouteCollection)
- Prefer Fluent ORM with database migrations
- Use middleware for auth, error handling, logging
- Validate all input with Vapor's Validation API
- Use environment variables for configuration via dotenv

## Testing Rules
- Write tests using XCTest or Swift Testing framework
- Use test doubles (protocol mocks) rather than inheritance mocks
- Test async code with `await` and `XCTestExpectation`
- Achieve minimum 80% coverage on business logic
- Write performance tests for critical paths
