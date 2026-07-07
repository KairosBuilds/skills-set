# Kairos — Multi-Agent Engineering Operating System

**Version 2.0.0** — Production-grade multi-agent coding ecosystem with **186 specialized agents** and **311 reusable skills** organized across **15 numbered execution tiers**.

A cohesive AI engineering operating system where every agent has a single, well-defined responsibility, skills are shared never duplicated, and execution flows through numbered pipeline tiers reflecting the actual development lifecycle.

---

## Execution Pipeline Architecture

Agents and skills are organized by **execution flow** — the order in which work actually happens — not alphabetically or by superficial category.

```
  00 Orchestrator   ─── entry point, routing, conflict resolution
  10 Intelligence   ─── AI/ML, prompt engineering, LLM evaluation
  15 Research       ─── domain research, technology comparison
  20 Planning       ─── feature, sprint, risk, task, roadmap planning
  25 Architecture   ─── system design, APIs, microservices, cloud
  30 Development    ─── coding, frontend (32), backend (31), mobile (33)
  35 Integrations   ─── GitHub, Slack, Shopify, Salesforce, Atlassian
  40 Quality        ─── testing (40), debugging (42), code review (45)
  50 Security       ─── audit, red team, web hunting, reconnaissance
  60 Operations     ─── DevOps (60), deployment (62), release (65), monitoring (67)
  70 Optimization   ─── performance (72), algorithm/build (70)
  75 Knowledge      ─── documentation, changelog, README generation
  80 Automation     ─── auto-fix, context management, workflow orchestration
  85 Repository     ─── repo analysis, dependency audit, workspace health
  90 Utilities      ─── PDF, Excel, slides, video, domain, productivity
```

---

## Agent-Category Map

| Tier | Category | Agents | Description |
|------|----------|--------|-------------|
| 00 | Orchestrator | 1 | Central coordinator — routes tasks, resolves conflicts, validates outputs |
| 10 | Intelligence | 10 | Prompt engineering, RAG, fine-tuning, deep research, LLM evaluation |
| 15 | Research | 5 | GitHub research, documentation research, technology comparison |
| 20 | Planning | 7 | Design thinking, feature, sprint, risk, roadmap, project, task planning |
| 25 | Architecture | 12 | System, solution, API, database, microservices, cloud, event-driven design |
| 30 | Development | 12 | Senior engineers, full-stack, backend, frontend, CLI, API, SDK, framework |
| 31 | Backend | 14 | Python, Node.js, Go, Rust, Java, C#, PHP, Rails, Django, FastAPI, NestJS, Spring, Kotlin, Laravel |
| 32 | Frontend | 10 | React, Vue, Angular, Next.js, TypeScript, CSS, animation, accessibility |
| 33 | Mobile | 7 | iOS, Android, Flutter, React Native, Kotlin, Swift, Appium |
| 35 | Integrations | 7 | GitHub, WordPress, Shopify, Salesforce, Atlassian, Slack, WeCom |
| 40 | Testing | 10 | Unit, integration, E2E, performance, regression, accessibility, QA |
| 42 | Debugging | 12 | Bug finder/fixer, crash analysis, race conditions, memory leaks, stack trace |
| 45 | Code Review | 12 | Code review, staff review, SOLID, design patterns, complexity, naming |
| 50 | Security | 10 | OWASP, secrets scanning, dependency audit, pen testing, supply chain |
| 60 | DevOps | 6 | CI/CD, Docker, K8s, Terraform, SRE, monitoring, observability |
| 62 | Deployment | 5 | Deployment automation, Docker, K8s, Terraform, CI/CD engineers |
| 65 | Release | 5 | Release management, migration planning, compatibility, semantic versioning |
| 67 | Monitoring | 4 | Observability, logging, telemetry, error monitoring specialists |
| 70 | Optimization | 2 | Algorithm optimization, build optimization |
| 72 | Performance | 8 | CPU, memory, bundle, network, caching, database, rendering optimizers |
| 75 | Documentation | 6 | README, API docs, code docs, changelogs, architecture documentation |
| 80 | Automation | 7 | Auto-fix, auto-setup, context management, verification, workflow optimization |
| 85 | Repository | 6 | Repo analysis, dependency analysis, workspace analysis, file structure, health |
| 90 | Utilities | 8 | PDF, Excel, slide deck, video download, web scraping, domain, invoice, SEO |

---

## Skill Domains (20 categories, 311 skills)

| Domain | Skills | Description |
|--------|--------|-------------|
| 10 Intelligence | 17 | Prompt engineering, RAG, deep research, LLM eval, fine-tuning |
| 20 Planning | 1 | Design thinking skill |
| 25 Architecture | 10 | API design, microservices, cloud, MCP builders, feature-forge |
| 31 Backend | 21 | Python, Go, Rust, Java, C#, PHP, Rails, NestJS, SQL, Spark, Kotlin |
| 32 Frontend | 9 | React, Vue, Angular, Next.js, TypeScript, game dev |
| 33 Mobile | 4 | Flutter, React Native, iOS, Appium |
| 35 Integrations | 12 | GitHub, Shopify, WordPress, Salesforce, Atlassian, Teams |
| 40 Testing | 18 | Playwright, Selenium, Cucumber, unit, E2E, integration, QA, webapp testing |
| 42 Code Quality | 12 | Code review, debugging, spec mining, adversarial review, the fool |
| 44 Database | 2 | SQL optimization, PostgreSQL |
| 46 Languages | 4 | Clojure, shadow-cljs, Clojure quality |
| 48 UI/UX | 6 | UI design, canvas, design systems, visual QA, artifacts builder |
| 50 Security | 87 | Reconnaissance, web-hunting (26), api-hunting (7), cloud-hunting (15), ai-security (1), application-security (4), red-team (18), defense (8), web3-crypto (2) |
| 60 DevOps | 28 | CI/CD, K8s, Terraform, Docker, PM2, monitoring, workspace tools |
| 75 Documentation | 11 | PDF, DOCX, XLSX, PPTX, slides, changelogs, brand guidelines |
| 80 OpenCode | 9 | Agent skills, config, diff management, session management, SDK |
| 82 Automation | 17 | Planner, executor, verifier, autofix, context optimization, token budget |
| 85 Workflow | 7 | Kanban state machine, transition validator, task executor, agile process, spec authoring (consolidated from 53) |
| 90 Productivity | 13 | SEO, i18n, file organization, domain names, competitive analysis, CLI demo |
| 92 Utilities | 23 | CLI, media, browser, data extraction, Twitter, YouTube, Bilibili, Feishu, downloaders |

---

## Routing System

The routing system follows the numbered execution tiers:

| Keyword Match | Primary Tier | Secondary |
|---------------|-------------|-----------|
| bug, error, crash, exception | 42 Debugging | 40 Testing |
| security, vulnerability, audit, hunt | 50 Security | 45 Code Review |
| performance, slow, optimize | 70 Optimization | 72 Performance |
| test, testing, coverage | 40 Testing | 42 Code Quality |
| documentation, docs, readme | 75 Documentation | 30 Development |
| deploy, release, ship | 60 DevOps | 65 Release |
| architect, design, structure | 25 Architecture | 20 Planning |
| review, refactor | 45 Code Review | 42 Code Quality |
| plan, sprint, roadmap | 20 Planning | 15 Research |
| frontend, ui, react, vue | 32 Frontend | 48 UI/UX |
| backend, api, server | 31 Backend | 25 Architecture |
| mobile, ios, android | 33 Mobile | 30 Development |
| docker, k8s, ci/cd | 60 DevOps | 62 Deployment |
| ai, ml, prompt, llm | 10 Intelligence | 15 Research |
| research, investigate | 15 Research | 10 Intelligence |
| monitor, observe, log | 67 Monitoring | 60 DevOps |
| config, setup, init | 80 Automation | 85 Repository |
| integration, github, slack | 35 Integrations | 30 Development |
| default (complex/unclear) | 00 Orchestrator | — |

---

## Standard Execution Pipelines

| Pipeline | Agent Flow (Tier Order) |
|----------|----------------------|
| **Full Feature** | 20 Planning → 25 Architecture → 30 Development → 31/32/33 Code → 35 Integrations → 40 Testing → 45 Code Review → 50 Security → 60 Operations → 75 Documentation |
| **Bug Fix** | 42 Debugging → 40 Testing (regression) → 45 Code Review → 65 Release |
| **Security Audit** | 50 Security → 45 Code Review (remediation) → 60 Operations (deploy) |
| **Performance Tuning** | 72 Performance → 70 Optimization → 40 Testing (benchmark) |
| **Deployment** | 60 DevOps → 62 Deployment → 65 Release → 67 Monitoring |
| **Full Pipeline** | All 15 tiers in numeric order |

---

## Architecture Layout

```
skills/
├── README.md              ← This file
├── AGENT.md               ← Ecosystem overview
├── EXECUTION_FLOW.md      ← Execution pipeline architecture
├── AGENTS_INDEX.md        ← Catalog of 186 agents (execution-flow ordered)
├── SKILLS_INDEX.md        ← Catalog of 311 skills (domain ordered)
├── SKILL_GRAPH.md         ← Skill dependency graph
├── WORKFLOWS.md           ← 10 standard workflows
├── ROUTING_RULES.md       ← Execution-flow routing decision tree
├── agents/                ← 186 agents (15 execution tiers)
│   ├── 00-orchestrator/   ← 1 agent (Orchestrator)
│   ├── 10-intelligence/   ← 10 agents
│   ├── 15-research/       ← 5 agents
│   ├── 20-planning/       ← 7 agents
│   ├── 25-architecture/   ← 12 agents
│   ├── 30-development/    ← 12 agents
│   ├── 31-backend/        ← 14 agents
│   ├── 32-frontend/       ← 10 agents
│   ├── 33-mobile/         ← 7 agents
│   ├── 35-integrations/   ← 7 agents
│   ├── 40-testing/        ← 10 agents
│   ├── 42-debugging/      ← 12 agents
│   ├── 45-code-review/    ← 12 agents
│   ├── 50-security/       ← 10 agents
│   ├── 60-devops/         ← 6 agents
│   ├── 62-deployment/     ← 5 agents
│   ├── 65-release/        ← 5 agents
│   ├── 67-monitoring/     ← 4 agents
│   ├── 70-optimization/   ← 2 agents
│   ├── 72-performance/    ← 8 agents
│   ├── 75-documentation/  ← 6 agents
│   ├── 80-automation/     ← 7 agents
│   ├── 85-repository/     ← 6 agents
│   └── 90-utilities/      ← 8 agents
├── skills/                ← 311 skills (20 domains)
│   ├── 10-intelligence/   ← 17 skills
│   ├── 20-planning/       ← 1 skill
│   ├── 25-architecture/   ← 10 skills
│   ├── 31-backend/        ← 21 skills
│   ├── 32-frontend/       ← 9 skills
│   ├── 33-mobile/         ← 4 skills
│   ├── 35-integrations/   ← 12 skills
│   ├── 40-testing/        ← 18 skills
│   ├── 42-code-quality/   ← 12 skills
│   ├── 44-database/       ← 2 skills
│   ├── 46-languages/      ← 4 skills
│   ├── 48-ui-ux/          ← 6 skills
│   ├── 50-security/       ← 87 skills (9 subcategories)
│   ├── 60-devops/         ← 28 skills
│   ├── 75-documentation/  ← 11 skills
│   ├── 80-opencode/       ← 9 skills
│   ├── 82-automation/     ← 17 skills
│   ├── 85-workflow/       ← 7 skills (consolidated from 53)
│   ├── 90-productivity/   ← 13 skills
│   └── 92-utilities/      ← 23 skills
├── commands/              ← Custom execution commands
├── knowledge/             ← Project knowledge base
└── shared/                ← Shared infrastructure
    ├── templates/         ← Agent creation template
    ├── configs/           ← Agent schema (JSON)
    ├── prompts/           ← System prompt template
    ├── standards/         ← Agent development standards
    ├── workflows/         ← Delegation workflow
    ├── schemas/           ← Metadata schema (YAML)
    └── utilities/         ← Skill resolver
```

---

## Consolidation Summary

| Area | Before | After | Change |
|------|--------|-------|--------|
| Workflow Skills | 53 | 4 | -49 (consolidated into state machine, validator, executor) |
| OpenCode Skills | 28 | 9 | -19 (merged: agent skills, skill mgmt, tools/mcp, config, diffs, sessions) |
| Security Skills | 87 | 87 | Reorganized into 9 subcategories (recon, web, api, cloud, ai, appsec, red-team, defense, web3) |
| Agent Categories | 24 | 15 | Execution-flow numbered (00-90) |
| Skill Domains | 19 | 20 | Renumbered with execution tiers |
| Total Skills | 376 | 311 | -65 (eliminated through deduplication) |

---

## Design Principles

1. **Single Responsibility** — Every agent has exactly one well-defined role
2. **Skill Reuse** — Agents share skills through a centralized registry; never duplicate logic
3. **Execution Flow** — Organization mirrors the development lifecycle, not alphabet
4. **Context Efficiency** — Agents receive only the context they need
5. **Hierarchical Coordination** — Numbered tiers reflect dependency ordering
6. **No Overlap** — Zero agent responsibility overlap; merged duplicates eliminated
7. **Production Ready** — Versioned, validated, documented, tested
8. **Acyclic Workflows** — No circular dependencies between tiers
9. **Quality Gated** — Automated validation on all agents and skills

---

## Quick Start

```bash
# Explore the agent catalog
cat AGENTS_INDEX.md

# Understand execution flow
cat EXECUTION_FLOW.md

# Check routing rules
cat ROUTING_RULES.md

# Browse skills
cat SKILLS_INDEX.md
```

---

## License

Copyright © 2026 Prateek Singh — Kairos
