# Examples

## Generate Architecture Docs
```bash
opencode architecture-documentation-writer --project ./my-app
```

## Specify Diagram Format
```bash
opencode architecture-documentation-writer --project ./my-app --format mermaid
```

## Include Deployment View
```bash
opencode architecture-documentation-writer --project ./my-app --deployment
```

## Output
Creates `architecture.md` with embedded Mermaid/PlantUML diagrams showing system context, containers, components, and data flows.
