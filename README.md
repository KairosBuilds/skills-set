# IRIS AI — Multi-Agent Skill Ecosystem

**Version 2.0.0** — Production-grade multi-agent engineering ecosystem with 160+ agents and 360+ reusable skills.

---

## Overview

This repository contains the complete agent and skill ecosystem for the IRIS AI platform. Agents are organized by specialization, share reusable skills through a centralized skill registry, and coordinate through a hierarchical routing system with an Orchestrator agent at the top.

Designed for AI-assisted software engineering across the full development lifecycle — from architecture and planning through coding, testing, security, deployment, and monitoring.

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/KairosBuilds/skill-set.git

# Browse agents
ls agents/

# Browse skills
ls skills/

# Read the agent catalog
cat AGENTS_INDEX.md

# Read the skill catalog
cat SKILLS_INDEX.md
```

---

## Architecture

```
skills/
├── AGENT.md              ← Ecosystem overview
├── AGENTS_INDEX.md       ← Catalog of 160+ agents
├── SKILLS_INDEX.md       ← Catalog of 360+ skills
├── SKILL_GRAPH.md        ← Skill dependency graph
├── WORKFLOWS.md          ← 10 standard workflows
├── ROUTING_RULES.md      ← Agent routing decision tree
├── agents/               ← 160+ agents (24 categories)
├── skills/               ← 360+ skills (19 categories)
├── commands/             ← Custom execution commands
├── knowledge/            ← Project knowledge base
└── shared/               ← Shared infrastructure
    ├── configs/          ← Agent schemas
    ├── prompts/          ← System prompt templates
    ├── schemas/          ← Metadata schemas
    ├── standards/        ← Agent development standards
    ├── templates/        ← Agent creation templates
    ├── utilities/        ← Skill resolver
    └── workflows/        ← Delegation workflows
```

---

## Agents (24 Categories)

| Category | Description | Agents |
|----------|-------------|--------|
| **Orchestration** | Task routing and coordination | Orchestrator |
| **Architecture** | System and solution design | Solution Architect, System Architect, API Designer, Cloud Architect, Microservices Architect, Database Architect |
| **Coding** | Core software engineering | Senior Software Engineer, Full Stack Engineer, Frontend/Backend Engineer, CLI Engineer, SDK Engineer |
| **AI** | AI/ML engineering | Prompt Engineer, RAG Architect, Deep Research Agent, Fine Tuning Specialist, LLM Evaluator |
| **Frontend** | Client-side development | React, Vue, Angular, Next.js, TypeScript, CSS, Animation, Responsive Design Engineers |
| **Backend** | Server-side development | Node.js, Python, Go, Rust, Java, C#, PHP, Rails, Kotlin, Django, FastAPI, NestJS Engineers |
| **Mobile** | Mobile development | iOS, Android, Flutter, React Native, Kotlin Mobile Engineers |
| **Security** | Security auditing | OWASP Specialist, Secrets Scanner, Security Auditor, Penetration Reviewer, Auth Reviewer, Supply Chain Auditor, API Security Auditor |
| **Testing** | Test engineering | Unit Test, E2E, Integration, Performance, QA, Accessibility, Regression Test Engineers |
| **Debugging** | Error diagnosis and fixing | Bug Finder, Bug Fixer, Crash Analyzer, Stack Trace Analyzer, Race Condition Detector, Memory Leak Detector |
| **Review** | Code and architecture review | Code Reviewer, Staff Engineer Reviewer, Architecture Reviewer, SOLID Validator, Refactoring Agent |
| **Performance** | Performance optimization | CPU, Memory, Bundle, Network, Caching, Database, Rendering Optimizers |
| **DevOps** | Infrastructure and operations | CI/CD, Docker, Kubernetes, Terraform, SRE, Monitoring Engineers |
| **Documentation** | Documentation generation | README Generator, API Docs Writer, Code Documenter, Changelog Generator |
| **Deployment** | Deployment automation | Deployment Engineer, K8s Engineer, Docker Engineer |
| **Planning** | Task and sprint planning | Task Planner, Sprint Planner, Project Planner, Roadmap Planner, Risk Planner |
| **Research** | Technology research | GitHub Research, Technology Comparison, Deep Research, Best Practice Research |
| **Repository** | Repository analysis | Repository Analyzer, Workspace Analyzer, File Structure Optimizer |
| **Release** | Release management | Release Manager, Migration Planner, Compatibility Checker, Semantic Version Manager |
| **Monitoring** | Observability | Observability Engineer, Monitoring Engineer, Error Monitoring, Logging Specialist |
| **Automation** | Workflow automation | Auto Fix, Auto Setup, Context Manager, Verification Agent, Workflow Optimizer, Token Optimizer |
| **Integrations** | Third-party integrations | WordPress, Shopify, Salesforce, Atlassian, GitHub, Teams |
| **Utilities** | Support utilities | PDF, Excel, Video Download, Slide Deck, CLI Developer |
| **Optimization** | Code and resource optimization | Algorithm Optimizer, Build Optimizer |

---

## Skills (19 Categories)

| Category | Count | Description |
|----------|-------|-------------|
| **security** | 87 | Security auditing, penetration testing, bug bounty, OSINT, vulnerability hunting |
| **workflow** | 52 | Agile workflow, Kanban state management, task status validation |
| **devops** | 27 | CI/CD, Docker, Kubernetes, Terraform, monitoring, SRE |
| **opencode** | 25 | OpenCode tooling, skill authoring, configuration management |
| **utilities** | 21 | Media tools, data extraction, browser tools, CLI tools |
| **backend** | 19 | Django, FastAPI, NestJS, Go, Rust, Python, Java, C#, PHP, Rails, Kotlin, SQL, Spark |
| **testing** | 18 | Playwright, Selenium, Cucumber, unit, integration, E2E, performance testing |
| **ai-ml** | 17 | Prompt engineering, RAG, fine-tuning, LLM evaluation, ML pipelines |
| **automation** | 17 | Auto-fix, planner, executor, verifier, context management |
| **productivity** | 13 | File organizer, SEO, i18n, domain name brainstorming |
| **integrations** | 12 | WordPress, Salesforce, Teams, Atlassian, GitHub, Shopify, WeCom |
| **documentation** | 11 | Code docs, API docs, PDF, PPTX, XLSX, slides, changelogs |
| **architecture** | 10 | System design, API design, cloud architecture, microservices, MCP |
| **code-quality** | 9 | Code review, debugging, spec mining, staff-level review |
| **frontend** | 9 | React, Vue, Angular, Next.js, TypeScript, JavaScript, game development |
| **ui-ux** | 5 | UI design, canvas, design systems, visual QA |
| **mobile** | 4 | Flutter, React Native, iOS, Android, Appium |
| **languages** | 4 | Clojure, shadow-cljs |
| **database** | 2 | SQL optimization, PostgreSQL |

---

## Routing System

Requests are classified by keywords and routed to the appropriate agent category:

- **Bugs/errors** → Debugging category
- **Security** → Security category
- **Performance** → Performance/Optimization
- **Testing** → Testing category
- **Documentation** → Documentation category
- **Deployment** → Deployment/Release
- **Architecture** → Architecture category
- **Review/refactor** → Review category
- **Planning** → Planning category
- **Research** → Research category
- **Frontend/UI** → Frontend category
- **Backend/API** → Backend category
- **Mobile/iOS/Android** → Mobile category
- **Docker/K8s/CI** → DevOps category
- **Default** → Orchestrator

See [ROUTING_RULES.md](./ROUTING_RULES.md) for the full decision tree.

---

## Standard Workflows

| # | Workflow | Agents Involved |
|---|----------|----------------|
| 1 | Full Feature Development | 10 agents — Planner → Repository Analyzer → Architecture Reviewer → Backend → Frontend → Security → Performance → Testing → Code Review → Documentation |
| 2 | Bug Fix | 6 agents — Bug Finder → Crash Analyzer → Bug Fixer → Regression Tester → Code Reviewer → Release Manager |
| 3 | Code Review | 5 agents — Code Reviewer → Security Auditor → Performance Optimizer → Architecture Reviewer → Staff Engineer Reviewer |
| 4 | Security Audit | 8 agents — Secrets Scanner → Dependency Auditor → OWASP → Auth Reviewer → API Security → Supply Chain → Pen Tester → Security Auditor |
| 5 | Performance Optimization | 8 agents — Profilers → CPU → Memory → Bundle → Network → Database → Caching → Algorithm Optimizers |
| 6 | Architecture Review | 6 agents — Repository Mapper → Solution Architect → System Architect → Microservices → Cloud → Database Architects |
| 7 | Testing Campaign | 8 agents — Unit → Integration → E2E → Coverage → Performance → Accessibility → Regression → QA |
| 8 | Documentation Generation | 6 agents — README → API Docs → Code Docs → Architecture Docs → Changelog → Comments |
| 9 | Deployment Pipeline | 7 agents — CI/CD → Docker → K8s → Infrastructure → Deployment → Monitoring → SRE |
| 10 | Research Investigation | 6 agents — GitHub Research → Docs Research → Technology Comparison → Best Practices → Deep Research → Architecture Research |

See [WORKFLOWS.md](./WORKFLOWS.md) for detailed workflow diagrams.

---

## Agent Structure

Each agent follows a strict structure with 12 files:

```
agents/<category>/<agent-name>/
├── AGENT.md                 # Agent definition
├── metadata.yaml            # Agent metadata
├── config.json              # Agent configuration
├── execution_rules.md       # Execution rules
├── workflow.md              # Agent workflow
├── examples.md              # Usage examples
├── dependencies.md          # Dependencies
├── supported_skills.md      # Associated skills
├── supported_languages.md   # Supported languages
├── supported_frameworks.md  # Supported frameworks
├── limitations.md           # Limitations
└── quality_checklist.md     # Quality gates
```

---

## Skill Structure

Each skill includes a `SKILL.md` definition file and optional subdirectories:

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

1. **Single Responsibility** — Every agent has exactly one clearly defined role
2. **Skill Reuse** — Agents share skills rather than duplicating logic
3. **Context Efficiency** — Agents receive only the context they need
4. **Hierarchical Coordination** — Orchestrator routes work to specialists
5. **No Overlap** — Agent responsibilities never overlap
6. **Production Ready** — Every agent is versioned, validated, and documented
7. **Acyclic Workflows** — All workflows must be acyclic
8. **Quality Gated** — Every agent must pass quality checks

---

## Quality Gates

- All agent files must be valid
- Skill references must resolve to existing skills
- No duplicate agent responsibilities
- All workflows must be acyclic
- Every agent must have compatible agents defined

---

## License

Copyright © 2026 Prateek Singh — KairosBuilds
