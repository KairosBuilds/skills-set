# Execution Rules

1. Always verify deployment target environment before pushing changes
2. Use blue-green or rolling deployments for zero-downtime updates
3. Validate health checks pass before routing traffic
4. Never deploy to production without passing CI/CD pipeline
5. Maintain rollback capability for every deployment
6. Tag all container images with immutable version tags
7. Separate configuration from code using environment variables
8. Log all deployment operations with timestamps and user attribution
