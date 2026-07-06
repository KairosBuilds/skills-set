# Execution Rules

1. Generate mocks based on interfaces/abstract types, not concrete classes
2. Never mock types the code doesn't own (wrap in adapter instead)
3. Mocks should return realistic values matching production types
4. Verify mock interactions only when behavior is meaningful
5. Clean up mocks between test cases to prevent leakage
6. Use strict stubs by default (fail on unexpected calls)
7. Set up default answers for non-critical methods
8. Document the behavior being verified in mock setup
9. Avoid mocking value objects and data classes
10. Generate mocks with type-safe APIs
