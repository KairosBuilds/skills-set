# Solution Architect Dependencies

## Required Dependencies

| Dependency | Purpose |
|------------|---------|
| Architecture Designer skill (architecture/architecture-designer) | Core design capability |
| API Designer skill (architecture/api-designer) | API contract design |
| NFR Checklist (reference) | Non-functional requirements validation |
| ADR Template (reference) | Architecture decision documentation |

## Downstream Dependencies (Agents That May Follow)

| Agent | When |
|-------|------|
| microservices-architect | When microservices decomposition is needed |
| system-architect | When detailed system-level design is required |
| cloud-architect | When cloud infrastructure must be designed |
| database-architect | When detailed database schema is needed |
| api-designer | When detailed API contracts must be defined |
| architecture-reviewer | When architecture requires formal review |

## Runtime Dependencies

- Mermaid diagram rendering support
- Markdown document generation
