# Event-Driven Architect Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Microservices Architect skill (architecture/microservices-architect) | Core event-driven patterns |

## Upstream Agents

| Agent | When |
|-------|------|
| microservices-architect | Provides service boundaries and communication needs |
| solution-architect | Provides overall solution context |
| system-architect | Provides system-level throughput and latency requirements |

## Downstream Agents

| Agent | When |
|-------|------|
| architecture-reviewer | Event architecture review |
| database-architect | When event store is needed |
| devops-engineer | Message broker deployment |
| monitoring-expert | Stream monitoring setup |

## Runtime Dependencies

- Mermaid diagram rendering
- Schema design tools
