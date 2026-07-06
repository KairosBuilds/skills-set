# IRIS-AI Skill Graph

Visual relationship map of all skill categories and their connections.

---

## Overview

```
IRIS-AI Skills (364 total across 19 categories)
|
+-- architecture (10)     +-- testing (18)     +-- automation (17)
+-- ai-ml (17)           +-- database (2)      +-- integrations (12)
+-- backend (19)         +-- devops (27)       +-- productivity (13)
+-- frontend (12)        +-- documentation (11) +-- utilities (21)
+-- mobile (4)           +-- code-quality (9)   +-- opencode (25)
+-- security (87)        +-- ui-ux (5)         +-- workflow (52)
                         +-- languages (4)
```

## Category Relationships

```
                          +----------+
   +--------------------->| OPENCODE |<----------------------+
   |                      +----------+                       |
   v                                                         v
+----------+   +--------+   +------+   +----------+   +-----------+
| WORKFLOW |-->| COMMON |-->| CODE |-->| TESTING  |-->| SECURITY  |
+----------+   | GROUND |   +------+   +----------+   +-----------+
               +--------+       |            |              |
                                 v            v              v
                          +----------+   +--------+   +-----------+
                          | BACKEND  |-->| DEVOPS |-->| DATABASE  |
                          +----------+   +--------+   +-----------+
                               |              |              |
                               v              v              v
                          +----------+   +--------+   +-----------+
                          | FRONTEND |   | AI-ML  |   | MOBILE    |
                          +----------+   +--------+   +-----------+
                               |              |              |
                               v              v              v
                          +----------+   +--------+   +-----------+
                          | UI-UX    |   | UTIL   |   | DOC       |
                          +----------+   +--------+   +-----------+
```

---

## Ai-ml (17)

- **Path:** `skills/ai-ml/`
- **Subdomains:** AI/ML Engineering, LLM Engineering, Prompt Engineering, RAG Systems, Fine-Tuning
- **Skills Count:** 17
- **Related Categories:** backend, utilities
- **All Skills:**
  - benchmark-due-diligence
  - content-research-writer
  - deep-research
  - fact-checker
  - fine-tuning-expert
  - image-enhancer
  - llm-eval-harness
  - llm-icon-finder
  - llm-wiki-setup
  - meeting-insights-analyzer
  - ml-pipeline
  - product-analysis
  - prompt-engineer
  - prompt-optimizer
  - promptfoo-evaluation
  - rag-architect
  - scrapling-skill

---

## Architecture (10)

- **Path:** `skills/architecture/`
- **Subdomains:** Architecture Design, System Design, API Design, Cloud Architecture, Microservices
- **Skills Count:** 10
- **Related Categories:** backend, frontend, database
- **All Skills:**
  - api-designer
  - architecture-designer
  - cloud-architect
  - codebase-mapper
  - feature-forge
  - graphql-architect
  - legacy-modernizer
  - mcp-builder
  - mcp-developer
  - microservices-architect

---

## Automation (17)

- **Path:** `skills/automation/`
- **Subdomains:** Workflow Automation, Task Automation, Context Management
- **Skills Count:** 17
- **Related Categories:** devops, workflow, productivity
- **All Skills:**
  - auto-repo-setup
  - autofix
  - break-edit-loop
  - context-compressor
  - context-fetch
  - context-health-monitor
  - emergency-confusion-reset
  - empirical-validation
  - executor
  - plan-checker
  - planner
  - repomix-unmixer
  - slack-gif-creator
  - task-atomicity-guard
  - token-budget
  - verifier
  - verify-resource-existence

---

## Backend (21)

- **Path:** `skills/backend/`
- **Subdomains:** Backend Development, API Development, Database Integration, Server Logic
- **Skills Count:** 21
- **Related Categories:** database, testing, security, devops
- **All Skills:**
  - cpp-pro
  - csharp-developer
  - django-expert
  - dotnet-core-expert
  - embedded-systems
  - fastapi-expert
  - golang-pro
  - java-architect
  - kotlin-specialist
  - laravel-specialist
  - nestjs-expert
  - pandas-pro
  - php-pro
  - python-pro
  - rails-expert
  - rust-engineer
  - spark-engineer
  - spring-boot-engineer
  - sql-pro
  - swift-expert
  - websocket-engineer

---

## Code-quality (9)

- **Path:** `skills/code-quality/`
- **Subdomains:** Code Review, Debugging, Static Analysis, Refactoring
- **Skills Count:** 9
- **Related Categories:** testing, security, automation
- **All Skills:**
  - code-review
  - code-reviewer
  - debugger
  - debugging-network-issues
  - debugging-wizard
  - named-persona-adversarial-review
  - spec-miner
  - staff-engineer-review
  - the-fool

---

## Database (2)

- **Path:** `skills/database/`
- **Subdomains:** Database Design, Query Optimization, Data Modeling
- **Skills Count:** 2
- **Related Categories:** backend, devops
- **All Skills:**
  - database-optimizer
  - postgres-pro

---

## Devops (27)

- **Path:** `skills/devops/`
- **Subdomains:** CI/CD, Infrastructure, Containerization, Monitoring, SRE
- **Skills Count:** 27
- **Related Categories:** security, testing, automation
- **All Skills:**
  - chaos-engineer
  - create-pm2-clj-config
  - create-pm2-ecosystem
  - devops-engineer
  - docker-compose-control
  - giga-workflow
  - kubernetes-specialist
  - marketplace-health-check
  - monitoring-expert
  - nx-integration
  - pm2-process-management
  - pm2-server-control
  - release-watcher
  - render-pm2-clj-config
  - sre-engineer
  - submodule-ops
  - terraform-engineer
  - terraform-skill
  - tunnel-doctor
  - windows-remote-desktop-connection-doctor
  - workspace-build
  - workspace-code-standards
  - workspace-commands
  - workspace-dependency-check
  - workspace-lint
  - workspace-navigation
  - workspace-typecheck

---

## Documentation (11)

- **Path:** `skills/documentation/`
- **Subdomains:** Technical Writing, API Documentation, Document Generation
- **Skills Count:** 11
- **Related Categories:** code-quality, productivity
- **All Skills:**
  - brand-guidelines
  - changelog-generator
  - code-documenter
  - docx
  - excel-automation
  - pdf
  - pptx
  - slides-creator
  - theme-factory
  - video-comparer
  - xlsx

---

## Frontend (9)

- **Path:** `skills/frontend/`
- **Subdomains:** Frontend Development, UI Components, State Management, TypeScript/JS
- **Skills Count:** 9
- **Related Categories:** ui-ux, testing, mobile
- **All Skills:**
  - angular-architect
  - fullstack-guardian
  - game-developer
  - javascript-pro
  - nextjs-developer
  - react-expert
  - typescript-pro
  - vue-expert
  - vue-expert-js

---

## Integrations (12)

- **Path:** `skills/integrations/`
- **Subdomains:** Platform Integration, API Integration, Third-Party Services
- **Skills Count:** 12
- **Related Categories:** backend, frontend, utilities
- **All Skills:**
  - atlassian-mcp
  - git-safety-check
  - github-contributor
  - github-integration
  - github-ops
  - internal-comms
  - notify-wecom
  - salesforce-developer
  - setup-notifications-via-wecom
  - shopify-expert
  - teams-channel-post-writer
  - wordpress-pro

---

## Languages (4)

- **Path:** `skills/languages/`
- **Subdomains:** Clojure, Lisp, Language-Specific Tools
- **Skills Count:** 4
- **Related Categories:** backend, frontend
- **All Skills:**
  - clojure-namespace-architect
  - clojure-quality
  - clojure-syntax-rescue
  - shadow-cljs-debug

---

## Mobile (4)

- **Path:** `skills/mobile/`
- **Subdomains:** Mobile Development, iOS, Android, Cross-Platform, App Testing
- **Skills Count:** 4
- **Related Categories:** frontend, testing
- **All Skills:**
  - appium-python-expert
  - flutter-expert
  - iOS-APP-developer
  - react-native-expert

---

## Opencode (25)

- **Path:** `skills/opencode/`
- **Subdomains:** OpenCode Tooling, Skill Authoring, Plugin Development, Config Management
- **Skills Count:** 25
- **Related Categories:** automation, utilities
- **All Skills:**
  - crafting-rules
  - opencode-agent-authoring
  - opencode-agent-file-generator
  - opencode-agents-skills
  - opencode-apply-reconstituted-diffs
  - opencode-command-authoring
  - opencode-configs
  - opencode-extract-diffs
  - opencode-model-variant-management
  - opencode-models-providers
  - opencode-plugin-authoring
  - opencode-plugins
  - opencode-reconstituter
  - opencode-recover-project
  - opencode-review-past-sessions
  - opencode-sdk
  - opencode-semantic-find-session
  - opencode-session-search
  - opencode-skill-creation
  - opencode-tool-authoring
  - opencode-tools-mcp
  - skill-authoring
  - skill-creator
  - skill-optimizing
  - skill-share

---

## Productivity (13)

- **Path:** `skills/productivity/`
- **Subdomains:** Developer Productivity, Research Tools, Content Creation
- **Skills Count:** 13
- **Related Categories:** utilities, automation
- **All Skills:**
  - arquiteto-de-empresa
  - cli-demo-generator
  - competitive-ads-extractor
  - competitors-analysis
  - developer-growth-analysis
  - domain-name-brainstormer
  - file-organizer
  - find-skills
  - i18n-expert
  - invoice-organizer
  - local-seo-manager
  - macos-cleaner
  - raffle-winner-picker

---

## Security (87)

- **Path:** `skills/security/`
- **Subdomains:** Security Auditing, Penetration Testing, Bug Bounty, Vulnerability Research, Secure Dev
- **Skills Count:** 87
- **Related Categories:** testing, devops, code-quality
- **All Skills:**
  - apk-redteam-pipeline
  - bb-local-toolkit
  - bb-methodology
  - bug-bounty
  - bugcrowd-reporting
  - cloud-iam-deep
  - cloudflare-troubleshooting
  - code-security-auditor
  - compliance-os
  - devsecops-free-auth
  - devsecops-free-cicd
  - devsecops-free-cloud
  - devsecops-free-discovery
  - devsecops-free-dns
  - devsecops-free-monitoring
  - devsecops-free-security
  - devsecops-free-storage
  - enterprise-vpn-attack
  - evidence-hygiene
  - github-sensitive-data-cleanup
  - hunt-api-misconfig
  - hunt-aspnet
  - hunt-ato
  - hunt-auth-bypass
  - hunt-brute-force
  - hunt-business-logic
  - hunt-cache-poison
  - hunt-cicd
  - hunt-cloud-misconfig
  - hunt-cors
  - hunt-csrf
  - hunt-deserialization
  - hunt-dispatch
  - hunt-dom
  - hunt-file-upload
  - hunt-graphql
  - hunt-grpc
  - hunt-host-header
  - hunt-http-smuggling
  - hunt-idor
  - hunt-k8s
  - hunt-laravel
  - hunt-ldap
  - hunt-lfi
  - hunt-llm-ai
  - hunt-mfa-bypass
  - hunt-misc
  - hunt-nextjs
  - hunt-nodejs
  - hunt-nosqli
  - hunt-ntlm-info
  - hunt-oauth
  - hunt-open-redirect
  - hunt-race-condition
  - hunt-rce
  - hunt-saml
  - hunt-session
  - hunt-sharepoint
  - hunt-source-leak
  - hunt-springboot
  - hunt-sqli
  - hunt-ssrf
  - hunt-ssti
  - hunt-subdomain
  - hunt-tls-network
  - hunt-websocket
  - hunt-xss
  - hunt-xxe
  - lead-research-assistant
  - m365-entra-attack
  - meme-coin-audit
  - mid-engagement-ir-detection
  - offensive-osint
  - okta-attack
  - osint-methodology
  - redteam-mindset
  - redteam-report-template
  - repomix-safe-mixer
  - report-writing
  - secure-code-guardian
  - security-arsenal
  - security-reviewer
  - supply-chain-attack-recon
  - triage-validation
  - vmware-vcenter-attack
  - web2-recon
  - web3-audit

---

## Testing (18)

- **Path:** `skills/testing/`
- **Subdomains:** Test Automation, E2E Testing, Unit Testing, Integration Testing, QA
- **Skills Count:** 18
- **Related Categories:** security, code-quality, devops
- **All Skills:**
  - lint-gate
  - playwright-automation-expert
  - playwright-cucumber-expert
  - playwright-expert
  - qa-expert
  - selenium-cucumber-expert
  - test-master
  - test-preservation
  - testing-bun
  - testing-clojure-cljs
  - testing-e2e
  - testing-general
  - testing-integration
  - testing-nx
  - testing-typescript-ava
  - testing-typescript-vitest
  - testing-unit
  - webapp-testing

---

## Ui-ux (5)

- **Path:** `skills/ui-ux/`
- **Subdomains:** UI Design, UX Research, Design Systems, Visual Design
- **Skills Count:** 5
- **Related Categories:** frontend, documentation
- **All Skills:**
  - artifacts-builder
  - canvas-design
  - design-style-picker
  - frontend-visual-qa
  - ui-designer

---

## Utilities (21)

- **Path:** `skills/utilities/`
- **Subdomains:** Utility Tools, Media Tools, Data Extraction, Browser Tools
- **Skills Count:** 21
- **Related Categories:** productivity, automation
- **All Skills:**
  - agent-decision-receipts
  - apology-action-protocol
  - bilibili-source
  - capture-screen
  - cli-developer
  - codex-image-gallery
  - douban-skill
  - download-gemini-images
  - feishu-doc-scraper
  - gemini-history-analyzer
  - ima-copilot
  - local-codex
  - lsp-server-integration
  - mcp-server-integration
  - openclaw
  - openclaw-model-switch
  - twitter-reader
  - video-downloader
  - webring-site
  - wps-doc-scraper
  - youtube-downloader

---

## Workflow (52)

- **Path:** `skills/workflow/`
- **Subdomains:** Agile Workflow, Kanban, Task Management
- **Skills Count:** 52
- **Related Categories:** automation, productivity
- **All Skills:**
  - agile-process
  - kanban-state-backlog
  - kanban-state-document
  - kanban-state-done
  - kanban-state-icebox
  - kanban-state-in-progress
  - kanban-state-review
  - kanban-state-todo
  - spec-authoring
  - update-task-status
  - validate-accepted-to-breakdown
  - validate-accepted-to-icebox
  - validate-blocked-to-breakdown
  - validate-breakdown-to-blocked
  - validate-breakdown-to-icebox
  - validate-breakdown-to-ready
  - validate-breakdown-to-rejected
  - validate-document-to-done
  - validate-document-to-in_review
  - validate-icebox-to-incoming
  - validate-in_progress-to-breakdown
  - validate-in_progress-to-in_review
  - validate-in_progress-to-todo
  - validate-in_review-to-breakdown
  - validate-in_review-to-in_progress
  - validate-in_review-to-testing
  - validate-in_review-to-todo
  - validate-incoming-to-accepted
  - validate-incoming-to-icebox
  - validate-incoming-to-rejected
  - validate-ready-to-breakdown
  - validate-ready-to-todo
  - validate-rejected-to-icebox
  - validate-task-status
  - validate-testing-to-document
  - validate-testing-to-in_progress
  - validate-testing-to-in_review
  - validate-todo-to-breakdown
  - validate-todo-to-in_progress
  - work-on-accepted-task
  - work-on-blocked-task
  - work-on-breakdown-task
  - work-on-document-task
  - work-on-done-task
  - work-on-icebox-task
  - work-on-in_progress-task
  - work-on-in_review-task
  - work-on-incoming-task
  - work-on-ready-task
  - work-on-rejected-task
  - work-on-testing-task
  - work-on-todo-task

---

*Auto-generated skill graph. Last built: 2026-07-06 20:55*
