# Repository Mapper Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Codebase Mapper skill (architecture/codebase-mapper) | Core codebase analysis capability |

## Upstream Agents

| Agent | When |
|-------|------|
| solution-architect | When architecture mapping is part of larger analysis |
| dependency-architect | When dependency analysis needs deeper investigation |
| legacy-modernizer | When mapping legacy codebase for migration |

## Downstream Agents

| Agent | When |
|-------|------|
| dependency-architect | For deeper dependency chain analysis |
| legacy-modernizer | When mapping reveals need for modernization |
| architecture-reviewer | For architecture boundary validation |
| development agents | For implementing refactoring suggestions |

## Runtime Dependencies

- Source code access (read-only)
- Mermaid or Graphviz for visualization
- Package manager manifest parsing (package.json, Cargo.toml, etc.)
