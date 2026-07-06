# Kairos AI � Agents Index

**Version 2.0.0** � Complete catalog of all specialized agents in the multi-agent coding system.

Last updated: 2026-07-06 | Total agents: 182
| # | Agent Name | Category | Priority | Cost | Status | Languages | Frameworks |
|---|-----------|----------|----------|------|--------|-----------|------------|
| 1 | Accessibility Engineer | frontend | medium | low | stable | ARIA attributes use kebab-case (`aria-label`, `aria-describedby`), WAI-ARIA 1.2 specification compliance, HTML semantic elements over ARIA whenever possible | **axe-core**: Run with `@axe-core/playwright` for E2E a11y; configure to WCAG 2.2 AA, **React Aria**: Use over custom ARIA when possible; follows WAI-ARIA patterns by default, **Lighthouse**: Check a11y score; use as baseline, not sole verification |
| 2 | Accessibility Tester | testing | medium | low | stable |  |  |
| 3 | Agent Builder | ai | high | medium | production | All |  |
| 4 | Ai Workflow Designer | ai | high | medium | stable |  |  |
| 5 | Algorithm Optimizer | optimization | medium | medium | stable | All | All |
| 6 | Android Engineer | mobile | high | high | production | All |  |
| 7 | Angular Engineer | frontend | high | medium | production | All | **Angular CLI**: Use `ng generate` for scaffolding; `ng build --strict` for production, **NgRx**: Feature states with lazy loading; `createAction`, `createReducer`, `createEffect`, **Angular Material**: Tree-shakeable imports only; custom theming with Material mixins |
| 8 | Animation Engineer | frontend | medium | low | stable | TypeScript for typed variant objects and animation configs, CSS custom properties for animation timing variables, JSX for Framer Motion code | **Framer Motion**: `animate={x}` over `transition` objects; variants for state machines, **GSAP**: `gsap.context()` for React scoping; cleanup in `useEffect` return, **R3F**: `useFrame(state, delta)` over `performance.now()`; adaptive DPR for performance |
| 9 | Api Designer | architecture | high | medium | production | All |  |
| 10 | Api Documentation Writer | documentation | medium | low | stable | All |  |
| 11 | Api Engineer | coding | "high" | "medium" | "production" |  |  |
| 12 | Api Security Auditor | security | high | high | production | All |  |
| 13 | Appium Engineer | mobile | medium | medium | stable |  | All |
| 14 | Architecture Documentation Writer | documentation | medium | low | stable | All |  |
| 15 | Architecture Research Agent | research | medium | low | stable | All | All |
| 16 | Architecture Reviewer | architecture | high | medium | production | All | All |
| 17 | Atlassian Integration Agent | integrations | high | medium | production | All |  |
| 18 | Authentication Reviewer | security | critical | high | production | All | All |
| 19 | Authorization Reviewer | security | critical | high | production | All |  |
| 20 | Auto Fix Agent | automation | high | medium | production | All | All |
| 21 | Auto Setup Agent | automation | high | low | production | All | All |
| 22 | Backend Engineer | coding | "critical" | "high" | "production" |  |  |
| 23 | Benchmark Engineer | ai | medium | high | stable |  |  |
| 24 | Best Practice Research Agent | research | medium | low | stable | All | All |
| 25 | Bug Finder | debugging | critical | high | production | All | All |
| 26 | Bug Fixer | debugging | critical | high | production | All | All |
| 27 | Build Optimizer | optimization | high | medium | production |  |  |
| 28 | Bundle Optimizer | performance | high | medium | production | All |  |
| 29 | Caching Optimizer | performance | high | medium | production | All |  |
| 30 | Changelog Generator | documentation | low | low | stable | All |  |
| 31 | Cicd Engineer | deployment | critical | high | production |  |  |
| 32 | Clean Code Auditor | review | high | medium | production | All | All |
| 33 | Cli Engineer | coding | "medium" | "medium" | "stable" |  |  |
| 34 | Cloud Architect | architecture | high | high | production |  |  |
| 35 | Cloud Security Reviewer | security | high | high | production |  |  |
| 36 | Code Completer | coding | "high" | "medium" | "production" | All | All |
| 37 | Code Documenter | documentation | medium | low | stable |  |  |
| 38 | Code Reviewer | review | critical | high | production | All | All |
| 39 | Comment Generator | documentation | low | low | stable |  |  |
| 40 | Compatibility Checker | release | high | medium | production | All |  |
| 41 | Complexity Analyzer | review | medium | low | stable | All | All |
| 42 | Concurrency Debugger | debugging | high | high | production | All | **Go** — goroutines, channels, select, sync.Mutex, sync.WaitGroup, sync.Pool, **Rust** — std::thread, Tokio, async-std, rayon, crossbeam, parking_lot, **Java** — Thread, ExecutorService, CompletableFuture, CountDownLatch, CyclicBarrier, Phaser, ForkJoinPool |
| 43 | Configuration Auditor | repository | medium | low | stable | JSON, YAML, TOML | All |
| 44 | Context Manager | automation | high | medium | production | All | All |
| 45 | Coverage Analyzer | testing | high | low | production | All | All |
| 46 | Cpu Optimizer | performance | high | high | production |  |  |
| 47 | Crash Analyzer | debugging | critical | high | production | All | All |
| 48 | Csharp Engineer | backend | "high" | "medium" | "production" |  |  |
| 49 | Css Specialist | frontend | medium | low | stable | CSS: Modern layout with Grid and Flexbox; `:where()`, `:is()`, `has()` selectors, SCSS: `@use` over `@import`; limited nesting; meaningful partial naming, Tailwind: Configure in `tailwind.config.js`; use `@apply` sparingly for shared component styles | **Tailwind**: Configure design tokens in theme.extend; purge unused classes; use `@apply` for shared component styles only, **Bootstrap**: Use utility classes over Sass customization; rely on CSS variables for theming, **Styled Components**: Co-locate styles with components; use transient props (`$prop`) to avoid passing to DOM |
| 50 | Database Architect | architecture | high | high | production | All |  |
| 51 | Database Engineer | coding | "high" | "medium" | "production" |  |  |
| 52 | Database Optimizer | performance | high | high | production | All |  |
| 53 | Dead Code Remover | review | medium | low | stable | All | All |
| 54 | Deep Research Agent | ai | high | high | production | All | All |
| 55 | Dependency Analyzer | repository | high | medium | production | All | npm, pip, cargo |
| 56 | Dependency Architect | architecture | high | medium | production |  |  |
| 57 | Dependency Auditor | security | high | medium | production | All |  |
| 58 | Deployment Engineer | deployment | critical | high | production |  |  |
| 59 | Design Pattern Advisor | review | medium | low | stable | All |  |
| 60 | Desktop Engineer | coding | "medium" | "medium" | "stable" |  |  |
| 61 | Devops Engineer | devops | critical | high | production |  |  |
| 62 | Django Engineer | backend | "high" | "medium" | "production" |  |  |
| 63 | Docker Engineer | deployment | critical | medium | production |  |  |
| 64 | Documentation Research Agent | research | medium | low | stable | All | All |
| 65 | Domain Name Agent | utilities | low | low | stable | All | All |
| 66 | Duplicate Code Detector | review | medium | low | stable | All | All |
| 67 | E2e Test Engineer | testing | critical | high | production |  |  |
| 68 | Edge Case Analyzer | debugging | medium | low | stable | All | All |
| 69 | Error Monitoring Specialist | monitoring | high | medium | production | All | All |
| 70 | Event Driven Architect | architecture | high | high | production |  |  |
| 71 | Excel Agent | utilities | low | low | stable |  |  |
| 72 | Fact Checker | ai | medium | low | stable | All | All |
| 73 | Fastapi Engineer | backend | "high" | "medium" | "production" |  |  |
| 74 | Feature Planner | planning | high | medium | production | All | All |
| 75 | File Organizer | automation | low | low | stable | All | All |
| 76 | File Structure Optimizer | repository | medium | low | stable | All | All |
| 77 | Fine Tuning Specialist | ai | high | high | production |  |  |
| 78 | Flutter Engineer | mobile | high | medium | production | All |  |
| 79 | Framework Engineer | coding | "high" | "high" | "production" | All | All |
| 80 | Frontend Engineer | coding | "critical" | "high" | "production" | All |  |
| 81 | Full Stack Engineer | coding | "critical" | "high" | "production" |  |  |
| 82 | Github Integration Agent | integrations | high | medium | production | All |  |
| 83 | Github Research Agent | research | medium | low | stable | All | GitHub API, GitHub GraphQL API, GitHub Actions (research only) |
| 84 | Go Engineer | backend | "high" | "medium" | "production" |  |  |
| 85 | Graphql Architect | architecture | high | medium | production |  |  |
| 86 | Infrastructure Engineer | devops | critical | high | production |  |  |
| 87 | Integration Test Engineer | testing | high | high | production |  | All |
| 88 | Invoice Organizer | utilities | low | low | stable | All | All |
| 89 | Ios Engineer | mobile | high | high | production | All |  |
| 90 | Java Engineer | backend | "high" | "medium" | "production" |  |  |
| 91 | Kotlin Engineer | backend | "high" | "medium" | "production" |  |  |
| 92 | Kotlin Mobile Engineer | mobile | high | medium | production | All |  |
| 93 | Kubernetes Engineer | deployment | critical | high | production |  |  |
| 94 | Laravel Engineer | backend | "high" | "medium" | "production" |  |  |
| 95 | Legacy Modernizer | architecture | high | high | production | All |  |
| 96 | Library Engineer | coding | "high" | "medium" | "production" |  |  |
| 97 | Llm Evaluator | ai | high | high | production |  |  |
| 98 | Local Seo Manager | utilities | low | low | stable | All |  |
| 99 | Logging Specialist | monitoring | medium | low | stable | All |  |
| 100 | Logic Error Detector | debugging | high | high | production | All | All |
| 101 | Memory Leak Detector | debugging | high | high | production | All | All |
| 102 | Memory Optimizer | performance | high | high | production | All | All |
| 103 | Microservices Architect | architecture | high | high | production |  |  |
| 104 | Migration Planner | release | high | medium | production | All | All |
| 105 | Mock Generator | testing | medium | low | stable |  |  |
| 106 | Monitoring Engineer | devops | high | medium | production | All |  |
| 107 | Naming Reviewer | review | low | low | stable | All | All |
| 108 | Nestjs Engineer | backend | "high" | "medium" | "production" |  |  |
| 109 | Network Optimizer | performance | high | medium | production | All |  |
| 110 | Nextjs Engineer | frontend | critical | medium | production | All | **Next.js**: `next.config.js` with proper image domains, redirects, headers, **Prisma/Drizzle**: Server-only imports (use `server-only` package), **NextAuth**: Route handler for `[...nextauth]`; middleware for session |
| 111 | Nodejs Engineer | backend | "critical" | "medium" | "production" |  |  |
| 112 | Observability Engineer | devops | high | medium | production | All |  |
| 113 | Observability Engineer | monitoring | high | medium | production | All |  |
| 114 | Orchestrator | orchestration | critical | high | production | All | Task routing engine, Context management system, Audit logging infrastructure |
| 115 | Owasp Specialist | security | critical | high | production | All |  |
| 116 | Pdf Agent | utilities | low | low | stable | All | All |
| 117 | Penetration Review Agent | security | high | high | production | All |  |
| 118 | Performance Optimizer | performance | critical | high | production | All | All |
| 119 | Performance Regression Detector | debugging | high | medium | production | All | **Lighthouse** — Full Lighthouse CI integration, **Web Vitals** — LCP, FID/INP, CLS analysis, **PageSpeed Insights** — Mobile and desktop metrics |
| 120 | Performance Tester | testing | high | high | production |  |  |
| 121 | Php Engineer | backend | "high" | "medium" | "production" |  |  |
| 122 | Project Planner | planning | high | medium | production | All | All |
| 123 | Prompt Engineer | ai | critical | medium | production | All |  |
| 124 | Prompt Optimizer | ai | high | low | stable | All |  |
| 125 | Python Engineer | backend | "critical" | "medium" | "production" |  |  |
| 126 | Qa Engineer | testing | critical | high | production | All | All |
| 127 | Race Condition Detector | debugging | high | high | production | **Go** — Built-in race detector (-race flag), ThreadSanitizer, **Rust** — ThreadSanitizer (nightly), Send/Sync trait verification, **Java** — ThreadSanitizer, happens-before analysis, synchronized analysis | **Go** — goroutines, channels, sync primitives, **Rust** — std::thread, tokio, async-std, crossbeam, rayon, **Java** — java.util.concurrent, ExecutorService, ForkJoinPool |
| 128 | Rag Architect | ai | high | high | production |  |  |
| 129 | Rails Engineer | backend | "high" | "medium" | "production" |  |  |
| 130 | React Engineer | frontend | critical | medium | production | All | **Next.js**: Default to App Router; use `'use client'` sparingly, **Remix**: Use loader/action pattern for data; prefer form mutations, **Vite**: Configure path aliases in `vite.config.ts` |
| 131 | React Native Engineer | mobile | critical | high | production | All |  |
| 132 | Readme Generator | documentation | low | low | stable | All | All |
| 133 | Refactoring Agent | review | high | high | production | All | All |
| 134 | Regression Tester | testing | high | high | production | All | All |
| 135 | Release Engineer | devops | high | medium | production |  |  |
| 136 | Release Manager | release | critical | high | production | All |  |
| 137 | Rendering Optimizer | performance | high | medium | production |  |  |
| 138 | Repository Analyzer | repository | high | medium | production | All | Git, Git-based version control systems |
| 139 | Repository Health Checker | repository | medium | low | stable | All | Git, CI/CD (GitHub Actions, GitLab CI, Jenkins), Code quality platforms (SonarQube, CodeClimate) |
| 140 | Repository Mapper | architecture | high | medium | production |  |  |
| 141 | Responsive Design Engineer | frontend | medium | low | stable | CSS Grid for macro-layouts, Flexbox for micro-layouts, `clamp()` for fluid values, CSS custom properties for breakpoint-aware spacing and typography | All |
| 142 | Risk Planner | planning | high | medium | production | All | All |
| 143 | Roadmap Planner | planning | high | medium | production | All | All |
| 144 | Runtime Error Specialist | debugging | critical | medium | production | All | All |
| 145 | Rust Engineer | backend | "high" | "medium" | "production" |  |  |
| 146 | Salesforce Integration Agent | integrations | medium | medium | stable |  |  |
| 147 | Sdk Engineer | coding | "high" | "medium" | "production" |  |  |
| 148 | Secrets Scanner | security | critical | high | production | All |  |
| 149 | Security Auditor | security | critical | high | production | All |  |
| 150 | Semantic Version Manager | release | medium | low | stable | All |  |
| 151 | Senior Software Engineer | coding | "critical" | "high" | "production" | All | All |
| 152 | Shopify Integration Agent | integrations | medium | medium | stable |  |  |
| 153 | Slack Integration Agent | integrations | low | low | stable | All |  |
| 154 | Slide Deck Creator | utilities | low | low | stable |  |  |
| 155 | Solid Validator | review | high | medium | production | All | All |
| 156 | Solution Architect | architecture | critical | high | production | All |  |
| 157 | Spring Engineer | backend | "high" | "medium" | "production" |  |  |
| 158 | Sprint Planner | planning | high | medium | production | All | Agile, Scrum, Kanban |
| 159 | Sre Engineer | devops | critical | high | production | All |  |
| 160 | Stack Trace Analyzer | debugging | critical | medium | production | All | Node.js, Deno, Bun, JVM (OpenJDK, GraalVM, Android Runtime), .NET Runtime (CoreCLR, Mono) |
| 161 | Staff Engineer Reviewer | review | high | high | production | All | All |
| 162 | Style Enforcer | review | low | low | stable | All | All |
| 163 | Supply Chain Auditor | security | high | high | production | All |  |
| 164 | Swift Engineer | mobile | high | medium | production | All |  |
| 165 | System Architect | architecture | critical | high | production |  |  |
| 166 | Task Planner | planning | high | medium | production | All | All |
| 167 | Technology Comparison Agent | research | medium | low | stable | All | All |
| 168 | Telemetry Reviewer | monitoring | medium | low | stable | All |  |
| 169 | Terraform Engineer | deployment | critical | medium | production |  |  |
| 170 | Test Preservation Agent | testing | high | low | production | All | All |
| 171 | Token Optimizer | automation | medium | low | stable | All | All |
| 172 | Typescript Engineer | frontend | critical | medium | production | All | **tRPC**: Ensure proper procedure types; infer client types from server, **Prisma**: Use generated `Prisma` namespace types; create DTO types separate from Prisma types, **Zod**: Infer TypeScript types from zod schemas with `z.infer<typeof schema>` |
| 173 | Ui Polish Agent | frontend | high | low | stable | Tailwind utility classes for most styling, CSS custom properties for theme values, Framer Motion `motion` components for animations | All |
| 174 | Unit Test Engineer | testing | critical | high | production |  |  |
| 175 | Verification Agent | automation | high | medium | production | All | All |
| 176 | Video Download Agent | utilities | low | low | stable | All |  |
| 177 | Vue Engineer | frontend | high | medium | production | All | **Nuxt**: Use `useFetch`, `useAsyncData` for data fetching; auto-import composables; `definePageMeta` for route metadata, **Pinia**: Define stores with setup syntax (function form), not options form, **Vue Router**: Lazy load routes with dynamic imports |
| 178 | Web Scraping Agent | utilities | medium | low | stable |  |  |
| 179 | Wecom Integration Agent | integrations | low | low | stable | All |  |
| 180 | Wordpress Integration Agent | integrations | medium | medium | stable |  |  |
| 181 | Workflow Optimizer | automation | high | medium | production | All | All |
| 182 | Workspace Analyzer | repository | medium | low | stable | All | Nx, Turborepo, Lerna |

---

## Agent Categories

| Category | Agent Count | Description |
|----------|-------------|-------------|
| ai | 10 | AI/ML engineering agents |
| architecture | 12 | System and solution design agents |
| automation | 7 | Workflow automation agents |
| backend | 14 | Server-side development agents |
| coding | 12 | Core software engineering agents |
| debugging | 11 | Error diagnosis and fixing agents |
| deployment | 5 | Deployment automation agents |
| devops | 6 | Infrastructure and operations agents |
| documentation | 6 | Documentation generation agents |
| frontend | 10 | Client-side development agents |
| integrations | 7 | Third-party integration agents |
| mobile | 7 | Mobile application development agents |
| monitoring | 4 | Observability agents |
| optimization | 2 | Code and resource optimization agents |
| orchestration | 1 | Task routing and coordination agents |
| performance | 8 | Performance optimization agents |
| planning | 6 | Task and sprint planning agents |
| release | 4 | Release management agents |
| repository | 6 | Repository analysis agents |
| research | 5 | Technology research agents |
| review | 11 | Code and architecture review agents |
| security | 10 | Security auditing agents |
| testing | 10 | Test engineering agents |
| utilities | 8 | Support utility agents |

---

## Quick Reference

- **Total Agents**: 182
- **Categories**: 24
- **Status**: Production-ready
- **Orchestrator**: Central coordinator that routes tasks to specialists
- **See Also**: [ROUTING_RULES.md](./ROUTING_RULES.md) | [WORKFLOWS.md](./WORKFLOWS.md) | [SKILLS_INDEX.md](./SKILLS_INDEX.md)