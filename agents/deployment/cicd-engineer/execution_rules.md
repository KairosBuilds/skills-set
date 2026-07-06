# Execution Rules

1. All pipelines must include build, test, and lint stages
2. Production deployments require manual approval gate
3. Secrets must use CI/CD secret management, never hardcoded
4. Cache dependencies to optimize pipeline execution time
5. Fail fast: stop pipeline on first critical failure
6. Version all artifacts with unique build numbers
7. Notify team on pipeline failures
8. Clean up build artifacts and temporary resources after completion
