# Database Architect Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Postgres Pro skill (database/postgres-pro) | PostgreSQL-specific expertise |
| Database Optimizer skill (database/database-optimizer) | Query optimization expertise |

## Upstream Agents

| Agent | When |
|-------|------|
| solution-architect | Provides overall data architecture context |
| system-architect | Provides scalability and performance requirements |
| microservices-architect | Provides per-service database boundaries |

## Downstream Agents

| Agent | When |
|-------|------|
| architecture-reviewer | Data architecture review |
| devops-engineer | Database deployment and operations |

## Runtime Dependencies

- ERD/Mermaid diagram rendering
- SQL formatting tools
