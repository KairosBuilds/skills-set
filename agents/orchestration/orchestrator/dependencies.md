# Orchestrator Dependencies

## Required Dependencies

| Dependency | Version | Purpose |
|------------|---------|---------|
| Agent Registry | >= 1.0 | Agent capability discovery and routing |
| Task Queue | >= 2.0 | Subtask queuing and execution management |
| Context Store | >= 1.0 | Shared context across agent handoffs |
| Audit Logger | >= 1.0 | Interaction and conflict logging |

## Agent Dependencies

The orchestrator depends on the availability of these agent categories:

| Category | Agents | Dependency Type |
|----------|--------|----------------|
| Architecture | solution-architect, system-architect, architecture-reviewer, microservices-architect, cloud-architect, event-driven-architect, api-designer, database-architect, graphql-architect, repository-mapper, dependency-architect, legacy-modernizer | Routing |
| Development | (all coding agents) | Routing |
| Review | (all review agents) | Routing |
| Testing | (all testing agents) | Routing |
| DevOps | (all devops agents) | Routing |
| Security | (all security agents) | Routing |

## Runtime Dependencies

- Node.js >= 18 (for agent scripting)
- Available system memory >= 512MB
- Disk space for audit logs >= 100MB

## Optional Dependencies

- Monitoring dashboard (for orchestration metrics visualization)
- Notification service (for alerting on agent failures)
