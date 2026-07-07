# Architecture Reviewer Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Architecture Designer skill (architecture/architecture-designer) | Architecture evaluation capability |
| Code Reviewer skill (code-quality/code-reviewer) | Structured review and reporting |

## Upstream Agents (Designs Received From)

| Agent | When |
|-------|------|
| solution-architect | Review solution-level architecture |
| system-architect | Review system-level design |
| microservices-architect | Review microservices decomposition |
| cloud-architect | Review cloud architecture |
| api-designer | Review API design |
| database-architect | Review database schema design |
| graphql-architect | Review GraphQL schema design |
| legacy-modernizer | Review migration architecture |

## Downstream Agents

| Agent | When |
|-------|------|
| solution-architect | Architecture revision after review |
| orchestrator | When review reveals need for cross-agent coordination |
