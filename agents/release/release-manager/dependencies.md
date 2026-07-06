# Dependencies

## Internal Agents
- **migration-planner**: Required for database/schema migrations during releases
- **compatibility-checker**: Validates dependency compatibility before deployment
- **semantic-version-manager**: Calculates version bumps and git tags

## External Tools
- **Git**: Source control operations
- **CI/CD System**: Pipeline execution (GitHub Actions)
- **Container Registry**: Image storage and promotion
- **Deployment Tooling**: Kubernetes manifests, Helm charts

## Runtime Requirements
- Node.js 18+ for semantic-release
- Docker for container operations
- Access to deployment environments
