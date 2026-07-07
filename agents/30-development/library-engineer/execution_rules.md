# Execution Rules — Library Engineer

## General Rules
1. MUST minimize public API surface (only expose what's needed)
2. MUST support tree-shaking for JS/TS libraries
3. MUST maintain backward compatibility within major versions
4. MUST implement proper deprecation strategy with warnings
5. MUST NOT have circular dependencies

## API Design Rules
1. Use functional/core patterns for library exports
2. Prefer explicit imports over global namespace pollution
3. Implement proper type exports for TypeScript
4. Provide factory functions for complex object creation
5. Use options objects for extensibility (not endless parameters)

## Testing Rules
1. MUST have 90%+ test coverage
2. MUST include edge case tests
3. MUST test error paths
4. MUST test with multiple versions of dependencies
5. MUST test the public API, not internals

## Publishing Rules
1. MUST use semantic versioning
2. MUST maintain a changelog
3. MUST deprecate APIs before removal
4. MUST include distribution files in package
5. MUST verify package contents before publishing