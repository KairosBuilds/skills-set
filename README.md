# Kairos AI — Multi-Agent Coding System

**Version 2.0.0** — Production-grade multi-agent coding ecosystem with **182 specialized agents** and **364 reusable skills** across **24 categories**.

---

## Overview

A professional AI engineering operating system built for the full development lifecycle. Agents are organized by specialization, share reusable skills through a centralized registry, and coordinate through a hierarchical routing system led by a central Orchestrator.

```
Architecture → Planning → Coding → Review → Testing → Security → Deploy → Monitor
```

---

## Architecture

```
skills/
├── AGENT.md              ← Ecosystem overview
├── AGENTS_INDEX.md       ← Catalog of 182 agents
├── SKILLS_INDEX.md       ← Catalog of 364 skills
├── SKILL_GRAPH.md        ← Skill dependency graph
├── WORKFLOWS.md          ← 10 standard workflows
├── ROUTING_RULES.md      ← Agent routing decision tree
├── agents/               ← 182 agents (24 categories)
│   ├── orchestration/    ← 1 agent (Orchestrator)
│   ├── architecture/     ← 12 agents
│   ├── coding/           ← 13 agents
│   ├── ai/               ← 10 agents
│   ├── frontend/         ← 10 agents
│   ├── backend/          ← 14 agents
│   ├── mobile/           ← 7 agents
│   ├── security/         ← 10 agents
│   ├── testing/          ← 10 agents
│   ├── debugging/        ← 11 agents
│   ├── review/           ← 11 agents
│   ├── performance/      ← 10 agents
│   ├── devops/           ← 6 agents
│   ├── deployment/       ← 5 agents
│   ├── documentation/    ← 6 agents
│   ├── planning/         ← 6 agents
│   ├── research/         ← 5 agents
│   ├── repository/       ← 6 agents
│   ├── release/          ← 4 agents
│   ├── monitoring/       ← 4 agents
│   ├── automation/       ← 7 agents
│   ├── integrations/     ← 7 agents
│   ├── optimization/     ← 2 agents
│   └── utilities/        ← 8 agents
├── skills/               ← 364 skills (19 categories)
├── commands/             ← Custom execution commands
├── knowledge/            ← Project knowledge base
└── shared/               ← Shared infrastructure
    ├── templates/        ← Agent creation template
    ├── configs/          ← Agent schema (JSON)
    ├── prompts/          ← System prompt template
    ├── standards/        ← Agent development standards
    ├── workflows/        ← Delegation workflow
    ├── schemas/          ← Metadata schema (YAML)
    └── utilities/        ← Skill resolver
```

---

## Agent Categories

| Category | Agents | Description |
|----------|--------|-------------|
| **Orchestration** | 1 | Central coordinator — routes tasks, resolves conflicts, validates outputs |
| **Architecture** | 12 | System/solution design, microservices, cloud, APIs, databases |
| **Coding** | 13 | Senior engineers, full-stack, API, CLI, SDK, framework engineers |
| **AI** | 10 | Prompt engineering, RAG, fine-tuning, LLM evaluation, deep research |
| **Frontend** | 10 | React, Vue, Angular, Next.js, TypeScript, CSS, animation, a11y |
| **Backend** | 14 | Python, Node.js, Go, Rust, Java, C#, PHP, Rails, Django, FastAPI |
| **Mobile** | 7 | iOS, Android, Flutter, React Native, Kotlin, Swift, Appium |
| **Security** | 10 | OWASP, secrets scanning, dependency audit, pen testing, supply chain |
| **Testing** | 10 | Unit, integration, E2E, performance, regression, a11y, QA |
| **Debugging** | 11 | Bug finder/fixer, crash analysis, race conditions, memory leaks |
| **Review** | 11 | Code review, staff review, SOLID, design patterns, complexity |
| **Performance** | 10 | CPU, memory, bundle, network, caching, database, rendering |
| **DevOps** | 6 | CI/CD, Docker, K8s, Terraform, SRE, monitoring |
| **Deployment** | 5 | Deployment, CI/CD, Docker, K8s, Terraform engineers |
| **Documentation** | 6 | README, API docs, code docs, changelogs, architecture docs |
| **Planning** | 6 | Task, sprint, roadmap, project, feature, risk planners |
| **Research** | 5 | GitHub, documentation, technology comparison, best practices |
| **Repository** | 6 | Analysis, dependency, workspace, file structure, health |
| **Release** | 4 | Release management, migration, compatibility, semver |
| **Monitoring** | 4 | Observability, logging, telemetry, error monitoring |
| **Automation** | 7 | Auto-fix, auto-setup, context management, verification |
| **Integrations** | 7 | GitHub, WordPress, Shopify, Salesforce, Atlassian, WeCom, Slack |
| **Optimization** | 2 | Algorithm optimization, build optimization |
| **Utilities** | 8 | PDF, Excel, slide deck, video download, web scraping, SEO |

---

## Skills (19 Categories)

| Category | Count | Skills |
|----------|-------|--------|
| **security** | 87 | hunt-* (56), devsecops-* (8), osint, compliance, audit, cloud security |
| **workflow** | 52 | Kanban states, validations, agile process, task status |
| **devops** | 27 | CI/CD, K8s, Terraform, Docker, monitoring, PM2, workspace |
| **opencode** | 25 | Agent authoring, skill creation, configs, plugins, tools, MCP |
| **utilities** | 21 | CLI, media, browser, data extraction, Twitter, YouTube |
| **backend** | 19 | Python, Go, Rust, Java, C#, PHP, Rails, NestJS, SQL, Spark |
| **testing** | 18 | Playwright, Selenium, Cucumber, unit, E2E, integration, QA |
| **ai-ml** | 17 | Prompt engineering, RAG, fine-tuning, deep research, LLM eval |
| **automation** | 17 | Planner, executor, verifier, autofix, context optimization |
| **productivity** | 13 | SEO, i18n, file organization, domain names, competitive analysis |
| **integrations** | 12 | GitHub, Shopify, WordPress, Salesforce, Atlassian, Teams |
| **documentation** | 11 | PDF, DOCX, XLSX, PPTX, slides, changelogs, brand guidelines |
| **architecture** | 10 | API design, microservices, cloud, MCP builders, feature-forge |
| **code-quality** | 9 | Code review, debugging, spec mining, adversarial review |
| **frontend** | 9 | React, Vue, Angular, Next.js, TypeScript, game dev |
| **ui-ux** | 5 | UI design, canvas, design systems, visual QA |
| **mobile** | 4 | Flutter, React Native, iOS, Appium |
| **languages** | 4 | Clojure, shadow-cljs |
| **database** | 2 | SQL optimization, PostgreSQL |

---

## Routing System

```
Request → Orchestrator parses intent → Routes to specialist agent → Validates output
```

| Keyword Match | Category |
|---------------|----------|
| bug, error, crash, exception | Debugging |
| security, vulnerability, audit | Security |
| performance, slow, optimize | Performance / Optimization |
| test, testing, coverage | Testing |
| documentation, docs, readme | Documentation |
| deploy, release, ship | Deployment / Release |
| architect, design, structure | Architecture |
| review, refactor | Review |
| plan, sprint, roadmap | Planning |
| research, investigate | Research |
| monitor, observe, log | Monitoring |
| config, setup, init | Automation |
| frontend, ui, react, vue | Frontend |
| backend, api, server | Backend |
| mobile, ios, android | Mobile |
| docker, k8s, ci/cd | DevOps |
| default (complex/unclear) | Orchestrator |

See [ROUTING_RULES.md](./ROUTING_RULES.md) for the full decision tree with priority scoring and conflict resolution.

---

## Standard Workflows

| # | Workflow | Agent Pipeline |
|---|----------|----------------|
| 1 | **Full Feature Development** | 10 agents — Planner → Repository Analyzer → Architect → Backend → Frontend → Security → Performance → Testing → Review → Documentation |
| 2 | **Bug Fix** | 6 agents — Bug Finder → Crash Analyzer → Bug Fixer → Regression Tester → Code Reviewer → Release Manager |
| 3 | **Code Review** | 5 agents — Code Reviewer → Security Auditor → Performance Optimizer → Architecture Reviewer → Staff Engineer |
| 4 | **Security Audit** | 8 agents — Secrets Scanner → Dependency Auditor → OWASP → Auth Reviewer → API Security → Supply Chain → Pen Tester → Auditor |
| 5 | **Performance Optimization** | 8 agents — CPU → Memory → Bundle → Network → Database → Caching → Algorithm → Build Optimizers |
| 6 | **Architecture Review** | 6 agents — Repository Mapper → Solution Architect → System Architect → Microservices → Cloud → Database |
| 7 | **Testing Campaign** | 8 agents — Unit → Integration → E2E → Coverage → Performance → Accessibility → Regression → QA |
| 8 | **Documentation Generation** | 6 agents — README → API Docs → Code Docs → Architecture Docs → Changelog → Comments |
| 9 | **Deployment Pipeline** | 7 agents — CI/CD → Docker → K8s → Infrastructure → Deployment → Monitoring → SRE |
| 10 | **Research Investigation** | 6 agents — GitHub → Documentation → Technology Comparison → Best Practices → Deep Research → Architecture |

See [WORKFLOWS.md](./WORKFLOWS.md) for detailed pipeline diagrams.

---

## Agent Structure

Every agent includes 12 required files:

```
agents/<category>/<agent-name>/
├── AGENT.md                 # Agent definition with frontmatter metadata
├── metadata.yaml            # Structured metadata (version, status, priority, cost)
├── config.json              # Execution configuration
├── execution_rules.md       # When and how this agent executes
├── workflow.md              # Step-by-step workflow
├── examples.md              # Usage examples
├── dependencies.md          # Agent and system dependencies
├── supported_skills.md      # Skill references (validated against actual skills)
├── supported_languages.md   # Programming languages supported
├── supported_frameworks.md  # Frameworks supported
├── limitations.md           # Known limitations
└── quality_checklist.md     # Quality gates and validation
```

### Metadata Requirements

Each agent frontmatter includes:
- `name`, `version`, `status`, `priority`
- `execution_cost` (low/medium/high)
- `confidence_level` (experimental/stable/production)
- `owner` (ecosystem/category)
- `compatibility` (target platforms)

---

## Skill Structure

```
skills/<category>/<skill-name>/
├── SKILL.md                 # Skill definition
├── references/              # Reference materials
├── scripts/                 # Automation scripts
├── templates/               # Templates
└── assets/                  # Assets (images, fonts, etc.)
```

---

## Design Principles

1. **Single Responsibility** — Every agent has exactly one role
2. **Skill Reuse** — Agents share skills, never duplicate logic
3. **Context Efficiency** — Agents receive only needed context
4. **Hierarchical Coordination** — Orchestrator routes to specialists
5. **No Overlap** — Zero agent responsibility overlap
6. **Production Ready** — Versioned, validated, documented
7. **Acyclic Workflows** — No circular dependencies
8. **Quality Gated** — Automated validation on all agents

---

## Quality Gates

- All 182 agents have 12 required files
- All frontmatter metadata is complete (version, priority, cost, confidence, owner, compatibility)
- All skill references resolve to existing skills (364 skills in registry)
- No duplicate agent responsibilities
- All workflows are acyclic
- Every agent has compatible agents defined

---

## Shared Infrastructure

| Component | Location | Purpose |
|-----------|----------|---------|
| Agent Template | `shared/templates/AGENT_TEMPLATE.md` | Standard agent scaffolding |
| Agent Schema | `shared/configs/agent_schema.json` | JSON validation schema |
| Metadata Schema | `shared/schemas/agent_metadata_schema.yaml` | YAML metadata validation |
| System Prompt | `shared/prompts/SYSTEM_PROMPT_TEMPLATE.md` | Standard system prompt |
| Standards | `shared/standards/AGENT_STANDARDS.md` | Development guidelines |
| Delegation Workflow | `shared/workflows/DELEGATION_WORKFLOW.md` | Agent handoff protocol |
| Skill Resolver | `shared/utilities/SKILL_RESOLVER.md` | Skill reference resolution |

---

## Stats

| Metric | Value |
|--------|-------|
| Total Agents | 182 |
| Agent Categories | 24 |
| Total Skills | 364 |
| Skill Categories | 19 |
| Shared Infrastructure Files | 7 |
| Standard Workflows | 10 |
| Validation Pass Rate | 100% |

---

## License

Copyright © 2026 Prateek Singh — Kairos AI
