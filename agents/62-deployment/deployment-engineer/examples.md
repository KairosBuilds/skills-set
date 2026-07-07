# Examples

## Deploy Application
```bash
opencode deployment-engineer deploy --app my-app --env production
```

## Rollback
```bash
opencode deployment-engineer rollback --app my-app --version v1.2.0
```

## Configure Deployment Strategy
```bash
opencode deployment-engineer configure --app my-app --strategy blue-green
```

## Output
Configures and executes application deployments with monitoring, health checks, and rollback capability.
