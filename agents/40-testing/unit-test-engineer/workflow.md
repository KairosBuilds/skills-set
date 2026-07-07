# Workflow

1. Analyze source code to identify testable units
2. Identify dependencies and determine mocking strategy
3. Write test cases covering:
   - Happy path (expected inputs)
   - Edge cases (empty, null, boundary values)
   - Error handling (invalid inputs, exceptions)
4. Execute tests and verify all pass
5. Review code coverage report
6. Add missing test cases for uncovered branches
7. Run full suite to confirm no regressions
8. Commit tests alongside source changes
