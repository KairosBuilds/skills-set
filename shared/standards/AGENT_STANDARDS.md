# Agent Standards

## Naming Conventions
- Agent names use Title Case (e.g., "Code Reviewer")
- Directory names use kebab-case (e.g., "code-reviewer")
- File names use UPPER_SNAKE_CASE for constants, kebab-case for definitions
- Skill references use the format: `category/skill-name`

## File Structure
Every agent directory MUST contain:
```
agent-name/
├── AGENT.md          # Comprehensive agent definition (REQUIRED)
├── metadata.yaml     # Machine-readable metadata (REQUIRED)
├── config.json       # Agent configuration (REQUIRED)
├── execution_rules.md # Execution constraints (REQUIRED)
├── workflow.md       # Step-by-step workflow (REQUIRED)
├── examples.md       # Example usage (REQUIRED)
├── dependencies.md   # Dependencies on other agents/skills (REQUIRED)
├── supported_skills.md # Skills this agent can load (REQUIRED)
├── supported_languages.md # Languages supported (REQUIRED)
├── supported_frameworks.md # Frameworks supported (REQUIRED)
├── limitations.md    # Known limitations (REQUIRED)
└── quality_checklist.md # Quality validation criteria (REQUIRED)
```

## Metadata Requirements
Every agent must define the following metadata fields:
- name, description, purpose, version, status (experimental/stable/production)
- priority (low/medium/high/critical), execution_cost (low/medium/high)
- confidence_level (experimental/stable/production)
- owner, compatibility
- supported_languages, supported_frameworks, supported_platforms
- required_skills, optional_skills, dependencies
- compatible_agents, incompatible_agents

## Quality Gates
1. All files must exist and be valid
2. All skill references must point to existing skills
3. All agent references must point to existing agents
4. No duplicate agent names
5. No overlapping responsibilities
6. All dependencies must be acyclic
7. Every agent must have at least one compatible agent
8. Configuration must match JSON schema

## Versioning
- Follow semver (MAJOR.MINOR.PATCH)
- MAJOR: Breaking changes to agent interface
- MINOR: New capabilities, backward compatible
- PATCH: Bug fixes, documentation updates
