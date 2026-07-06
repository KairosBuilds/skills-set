# Execution Rules

1. Use Testcontainers for database/service dependencies
2. Never mock the component under test's immediate dependencies
3. Test real API contracts, not implementation details
4. Clean up test data and containers after each test
5. Use isolated databases per test run
6. Test error propagation between components
7. Validate request/response schemas in contract tests
8. Keep integration tests separate from unit tests
9. Tag slow tests for optional execution
10. Never write integration tests that overlap with unit tests
