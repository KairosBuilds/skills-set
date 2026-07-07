# Dependency Architect Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Codebase Mapper skill (architecture/codebase-mapper) | Core dependency analysis capability |

## Upstream Agents

| Agent | When |
|-------|------|
| repository-mapper | Provides initial codebase map |
| solution-architect | Provides intended architecture boundaries |

## Downstream Agents

| Agent | When |
|-------|------|
| architecture-reviewer | Dependency architecture review |
| legacy-modernizer | When dependency restructuring is part of modernization |
| development agents | For implementing dependency changes |

## Runtime Dependencies

- ESLint or similar for import rule definition
- Dependency analysis tools (Madge, depcheck, etc.)
