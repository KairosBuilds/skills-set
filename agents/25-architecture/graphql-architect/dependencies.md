# GraphQL Architect Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| GraphQL Architect skill (architecture/graphql-architect) | Core GraphQL design capability |

## Upstream Agents

| Agent | When |
|-------|------|
| api-designer | Provides API design context |
| solution-architect | Provides overall architecture context |
| microservices-architect | Provides service boundaries for federation |

## Downstream Agents

| Agent | When |
|-------|------|
| architecture-reviewer | GraphQL schema review |
| development agents | Schema implementation |
| database-architect | When resolver data fetching needs optimization |

## Runtime Dependencies

- GraphQL SDL specification
- Apollo Federation specification (if federated)
