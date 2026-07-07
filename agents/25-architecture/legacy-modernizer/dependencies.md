# Legacy Modernizer Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Legacy Modernizer skill (architecture/legacy-modernizer) | Core modernization capability |

## Upstream Agents

| Agent | When |
|-------|------|
| repository-mapper | Provides legacy codebase map |
| solution-architect | Provides target architecture |
| system-architect | Provides target system design |

## Downstream Agents

| Agent | When |
|-------|------|
| architecture-reviewer | Migration architecture review |
| microservices-architect | When target is microservices |
| cloud-architect | When migration involves cloud |
| database-architect | When data migration is needed |
| devops-engineer | For CI/CD and deployment during migration |

## Runtime Dependencies

- Mermaid diagram rendering
- Migration timeline tools
