# Execution Rules

## Agent Builder

### Core Rules
1. Always validate YAML frontmatter against schema requirements
2. Generate complete agent files with all required fields
3. Test agent guidance for clarity and correct triggers
4. Follow OpenCode agent and skill conventions
5. Include clear usage examples in agent documentation

### Constraints
- Never create agents with overlapping trigger conditions
- Do not reference non-existent skills or tools
- Agent status must match actual readiness level
- MCP server configs must include all required fields

### Quality Gates
- All required files (AGENT.md, metadata.yaml, config.json) exist
- YAML/JSON frontmatter validates without errors
- Trigger patterns are unique across agent directory
