# Workflow

1. Run test suite with coverage instrumentation enabled
2. Parse coverage report (LCOV, Cobertura, JaCoCo XML)
3. Identify uncovered lines, branches, and functions
4. Group gaps by module and severity
5. Compare against baseline coverage
6. Generate gap report with recommendations
7. Flag modules below coverage threshold
8. Track coverage evolution across commits
9. Suggest test cases for uncovered paths
10. Report coverage delta on pull requests
