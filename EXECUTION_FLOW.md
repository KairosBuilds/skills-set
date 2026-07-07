# Kairos — Execution Flow Architecture

**Version 2.0.0** — The entire agent ecosystem reorganized by execution pipeline.

## Architecture Philosophy

Agents and skills are organized by **execution flow** — the order in which work actually happens — not by superficial category or alphabet. Each numbered tier represents a phase in the development lifecycle.

`
  00 Orchestrator      (entry point, routing)
  10 Intelligence      (AI/ML, prompt engineering)
  15 Research           (domain research, technology comparison)
  20 Planning           (feature, sprint, risk, task planning)
  25 Architecture       (system, solution, API design)
  30 Development        (coding, frontend, backend, mobile)
  35 Integrations       (third-party service integration)
  40 Quality            (testing, debugging, code review)
  50 Security           (audit, vulnerability assessment)
  60 Operations         (DevOps, deployment, release, monitoring)
  70 Optimization       (performance, resource optimization)
  75 Knowledge          (documentation, changelog)
  80 Automation         (workflow automation, context management)
  85 Repository         (repo analysis, health checking)
  90 Utilities          (support tools, productivity)
`

## Execution Graph

Work flows through the system in phases, with feedback loops:

`
User Request
    |
    v
[00 Orchestrator] ----routes to appropriate phase--->
    |                                                   |
    v                                                   v
[10 Intelligence] -> [15 Research] -> [20 Planning]
    |                                                   |
    v                                                   |
[25 Architecture]                                       |
    |                                                   |
    v                                                   |
[30 Development] <-----> [35 Integrations]              |
    |                                                   |
    v                                                   |
[40 Quality] <---- feedback loop (debugging)            |
    |                                                   |
    v                                                   |
[50 Security]                                           |
    |                                                   |
    v                                                   |
[60 Operations] -> [70 Optimization] -> [75 Knowledge]  |
    |                                                   |
    v                                                   |
[80 Automation] -> [85 Repository] -> [90 Utilities]    |
    |                                                   |
    +---------------------------------------------------+
`

## Dependency Ordering

Each tier explicitly declares its dependencies:
- **Tier 00**: No dependencies (entry point)
- **Tier 10-20**: May depend on 00
- **Tier 25-35**: Depend on 20 (planning must precede architecture)
- **Tier 40**: Depend on 30 (code must exist before testing)
- **Tier 50**: Depend on 30 (code must exist before security review)
- **Tier 60**: Depend on 30, 35 (must build before deploying)
- **Tier 70**: Depend on 30, 40 (performance on built + tested code)
- **Tier 75-90**: Depend on all prior tiers

## Parallel Execution

Independent tiers can execute in parallel:
- **31 Backend** + **32 Frontend** + **33 Mobile**: Independent, can run concurrently
- **40 Testing** + **45 Code Review** + **42 Debugging**: Can run in parallel
- **60 DevOps** + **65 Release**: Sequential (release depends on devops)

## Ownership Model

Each tier has a designated owner (Prateek) who is responsible for:
1. Quality of agent definitions within the tier
2. Skill availability for the tier's agents
3. Cross-tier dependency management
4. Tier-specific index maintenance

## Routing Decision Matrix

| Request Type | Primary Tier | Secondary | Description |
|---|---|---|---|
| Bug/Error/Crash | 42 Debugging | 40 Testing | Diagnose and fix |
| Security/Vulnerability | 50 Security | 45 Code Review | Audit and patch |
| Performance/Slow | 70 Optimization | 40 Testing | Profile and optimize |
| Test/Coverage | 40 Testing | 42 Code Quality | Write/improve tests |
| Documentation/Docs | 75 Knowledge | 30 Development | Generate docs |
| Deploy/Release/Ship | 60 Operations | 65 Release | Package and ship |
| Architect/Design | 25 Architecture | 20 Planning | Design solution |
| Plan/Sprint/Roadmap | 20 Planning | 15 Research | Plan work |
| Frontend/UI | 32 Frontend | 48 UI/UX | Build UI |
| Backend/API | 31 Backend | 25 Architecture | Build API |
| Mobile/iOS/Android | 33 Mobile | 30 Development | Build mobile |
| AI/ML/Prompt | 10 Intelligence | 15 Research | AI engineering |
| DevOps/Docker/K8s | 60 DevOps | 62 Deployment | Infrastructure |
| Config/Setup/Init | 80 Automation | 85 Repository | Configure project |
| Research/Investigate | 15 Research | 10 Intelligence | Research topic |
| Monitor/Observe | 67 Monitoring | 60 DevOps | Add observability |