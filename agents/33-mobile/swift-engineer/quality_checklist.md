# Quality Checklist — Swift Engineer

## Build & Compilation
- [ ] `swift build` succeeds without warnings
- [ ] `swift test` passes all test cases
- [ ] `swiftlint` passes with zero violations
- [ ] Release build succeeds with optimizations
- [ ] Package.swift is well-formed with correct versions
- [ ] No force unwraps or implicitly unwrapped optionals

## Functional
- [ ] All public APIs have documentation comments
- [ ] Codable types handle edge cases (optional fields, null values)
- [ ] Error types are meaningful and provide recovery guidance
- [ ] Async functions handle cancellation properly
- [ ] Actors protect shared mutable state
- [ ] MainActor used correctly for UI updates
- [ ] Resource cleanup in defer blocks

## Performance
- [ ] No retain cycles (weak references where needed)
- [ ] Copy-on-write optimized for large value types
- [ ] Lazy properties for expensive computations
- [ ] JSON encoding/decoding performance profiled
- [ ] No unnecessary COW copies of arrays/dictionaries
- [ ] Server endpoints have appropriate timeout handling

## Concurrency
- [ ] Structured concurrency used over unstructured tasks
- [ ] Task cancellation handled in long-running operations
- [ ] Task priority appropriate for work type
- [ ] No synchronous blocking calls in async contexts
- [ ] Non-sendable types not passed across concurrency boundaries

## Code Quality
- [ ] Access modifiers appropriate (public/internal/private)
- [ ] Protocol-oriented design where appropriate
- [ ] No print statements in production code
- [ ] os_log for all logging (with privacy annotations)
- [ ] No large enums with raw values (use strings)
- [ ] Consistent error handling pattern across codebase
- [ ] Test coverage >= 80% on business logic
- [ ] Performance tests for critical paths

## Server-Side (if applicable)
- [ ] Routes validated with Vapor Validation API
- [ ] Database migrations are idempotent
- [ ] Middleware chain is correct (error, cors, auth)
- [ ] Environment configuration via dotenv
- [ ] Graceful shutdown handling
- [ ] Rate limiting configured for public endpoints
