# API Designer Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| API Designer skill (architecture/api-designer) | Core API design capability |

## Upstream Agents

| Agent | When |
|-------|------|
| solution-architect | Provides overall API strategy |
| microservices-architect | Provides service boundaries needing APIs |
| system-architect | Provides performance requirements |

## Downstream Agents

| Agent | When |
|-------|------|
| graphql-architect | When deeper GraphQL specialization is needed |
| architecture-reviewer | API design review |
| development agents | API implementation |

## Runtime Dependencies

- OpenAPI 3.1 specification schema
- GraphQL SDL tools
- Protobuf compiler reference
