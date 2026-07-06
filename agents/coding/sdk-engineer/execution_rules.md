# Execution Rules — SDK Engineer

## General Rules
1. MUST maintain consistent API surface across all language SDKs
2. MUST implement automatic retry with exponential backoff
3. MUST handle all error types with descriptive messages
4. MUST implement proper authentication handling
5. MUST support both sync and async patterns where applicable

## Design Rules
1. Follow language-specific conventions for naming and patterns
2. Use builder or options pattern for complex configuration
3. Implement fluent interfaces for chaining operations
4. Provide factory methods for common use cases
5. Implement proper serialization/deserialization

## Documentation Rules
1. MUST provide README with quick start guide
2. MUST document all public methods with examples
3. MUST provide migration guides for breaking changes
4. MUST include API reference documentation

## Quality Rules
1. MUST have 90%+ test coverage for core logic
2. MUST include integration tests against real API
3. MUST implement proper versioning (semver)
4. MUST have CI/CD for automated testing and publishing
5. MUST handle edge cases (network errors, timeouts, rate limiting)