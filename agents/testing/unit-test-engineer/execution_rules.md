# Execution Rules

1. Always read the source file before writing tests
2. Tests must be deterministic — no reliance on external state
3. Mock all external dependencies (network, filesystem, databases)
4. Follow AAA pattern: Arrange, Act, Assert
5. One logical assertion per test case
6. Use descriptive test names that explain the scenario
7. Never modify source code to make tests pass
8. Run the full test suite after adding new tests
9. Report coverage gaps as findings
10. Keep test files alongside source files (co-located)
