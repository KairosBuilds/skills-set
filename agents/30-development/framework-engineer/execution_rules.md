# Execution Rules — Framework Engineer

## General Rules
1. MUST maintain backward compatibility within major versions
2. MUST implement proper deprecation strategy with warnings
3. MUST document all public APIs comprehensively
4. MUST implement comprehensive error handling
5. MUST design for extensibility from the start

## Design Rules
1. Favor convention over configuration where appropriate
2. Implement plugin/extension points for customization
3. Use dependency injection for loose coupling
4. Provide sensible defaults for all configuration
5. Implement middleware/interceptor patterns for cross-cutting concerns

## Compatibility Rules
1. Major version = breaking changes only
2. Minor version = new features, backward compatible
3. Patch version = bug fixes only
4. Deprecate APIs for one full minor version before removal

## Testing Rules
1. MUST have > 80% test coverage
2. MUST include integration tests for framework flows
3. MUST test plugin API extensibility
4. MUST test with sample applications
5. MUST benchmark performance-critical paths