# Workflow

1. Identify external dependencies to mock (DB, API, filesystem)
2. Define mock interfaces based on source types
3. Generate mock implementations with sensible defaults
4. Configure expected behaviors and return values
5. Wire mocks into test subjects using dependency injection
6. Verify mock interactions match expected call patterns
7. Clean up mocks after test completion
8. Document mock setup for reusability across tests
