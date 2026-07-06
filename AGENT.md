---
name: "IRIS AI Multi-Agent Ecosystem"
version: "2.0.0"
status: "production"
priority: "critical"
owner: "ecosystem/architecture"
last_updated: "2026-07-06"
---

# IRIS AI — Multi-Agent Engineering Ecosystem

## Architecture Overview
The `.opencode/` directory implements a production-grade multi-agent ecosystem.
Agents are organized by specialization, share reusable skills, and coordinate
through a central Orchestrator agent.

## Design Principles
1. **Single Responsibility**: Every agent has exactly one clearly defined role
2. **Skill Reuse**: Agents share skills rather than duplicating logic
3. **Context Efficiency**: Agents receive only the context they need
4. **Hierarchical Coordination**: Orchestrator routes work to specialists
5. **No Overlap**: Agent responsibilities never overlap
6. **Production Ready**: Every agent is versioned, validated, and documented

## Directory Map
```
.opencode/
├── AGENT.md              ← This file — ecosystem overview
├── AGENTS_INDEX.md       ← Complete agent catalog
├── SKILLS_INDEX.md       ← Complete skill catalog (auto-generated)
├── SKILL_GRAPH.md        ← Skill dependency graph (auto-generated)
├── WORKFLOWS.md          ← Standard workflows
├── ROUTING_RULES.md      ← Agent routing rules
├── agents/               ← Agent definitions (24 categories)
├── shared/               ← Shared infrastructure
├── skills/               ← 364 reusable skills (19 categories)
├── commands/             ← Custom commands
└── knowledge/            ← Project knowledge base
```

## Agent Categories
| Category | Directory | Focus |
|----------|-----------|-------|
| Orchestration | agents/orchestration/ | Task routing and coordination |
| Architecture | agents/architecture/ | System and solution design |
| Coding | agents/coding/ | Core software engineering |
| Backend | agents/backend/ | Server-side development |
| Frontend | agents/frontend/ | Client-side development |
| Mobile | agents/mobile/ | Mobile application development |
| AI | agents/ai/ | AI/ML engineering |
| Debugging | agents/debugging/ | Error diagnosis and fixing |
| Review | agents/review/ | Code and architecture review |
| Security | agents/security/ | Security auditing |
| Testing | agents/testing/ | Test engineering |
| Performance | agents/performance/ | Performance optimization |
| Optimization | agents/optimization/ | Code and resource optimization |
| Documentation | agents/documentation/ | Documentation generation |
| Deployment | agents/deployment/ | Deployment automation |
| DevOps | agents/devops/ | Infrastructure and operations |
| Planning | agents/planning/ | Task and sprint planning |
| Research | agents/research/ | Technology research |
| Repository | agents/repository/ | Repository analysis |
| Release | agents/release/ | Release management |
| Monitoring | agents/monitoring/ | Observability |
| Automation | agents/automation/ | Workflow automation |
| Integrations | agents/integrations/ | Third-party integrations |
| Utilities | agents/utilities/ | Support utilities |

## Skill Categories
| Category | Count | Focus |
|----------|-------|-------|
| ai-ml | 17 | AI/ML workflows |
| architecture | 10 | Architecture design |
| automation | 17 | Process automation |
| backend | 19 | Backend frameworks |
| code-quality | 9 | Code analysis |
| database | 2 | Database optimization |
| devops | 27 | Infrastructure |
| documentation | 11 | Documentation |
| frontend | 9 | Frontend frameworks |
| integrations | 12 | Third-party tools |
| languages | 4 | Language-specific |
| mobile | 4 | Mobile development |
| opencode | 25 | OpenCode configuration |
| productivity | 13 | Productivity tools |
| security | 87 | Security testing |
| testing | 18 | Test automation |
| ui-ux | 5 | Design systems |
| utilities | 21 | General utilities |
| workflow | 52 | Workflow automation |

## Quality Gates
1. `npm run typecheck` must pass before commit
2. All agent files must be valid
3. Skill references must resolve to existing skills
4. No duplicate agent responsibilities
5. All workflows must be acyclic
6. Every agent must have compatible agents defined
