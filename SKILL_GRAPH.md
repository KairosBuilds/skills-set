# Kairos — Skill Graph

Visual relationship map of all skill categories and their connections.

---

## Overview

```
Kairos Skills (364 total across 19 categories)
│
├── security (87)       ├── testing (18)       ├── automation (17)
├── workflow (52)       ├── ai-ml (17)         ├── integrations (12)
├── devops (27)         ├── backend (19)       ├── productivity (13)
├── opencode (25)       ├── frontend (12)      ├── utilities (21)
├── utilities (21)      ├── documentation (11) ├── architecture (10)
├── code-quality (9)    ├── ui-ux (5)          ├── mobile (4)
├── languages (4)       ├── database (2)
```

## Category Relationships

```
                    +----------+
   +--------------->| OPENCODE |<-------------------+
   |                +----------+                    |
   v                                                 v
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

## Category Details

| Category | Count | Key Skills | Dependencies |
|----------|-------|------------|-------------|
| security | 87 | hunt-* (56), devsecops-* (8), osint, compliance | testing, backend |
| workflow | 52 | kanban-state-* (8), validate-* (28), work-on-* (13) | opencode |
| devops | 27 | devops-engineer, k8s, terraform, docker, monitoring | backend, database |
| opencode | 25 | skill-authoring, agent-authoring, config, plugins | none |
| utilities | 21 | cli, youtube, feishu, bilibili, twitter, pdf, xlsx | backend |
| backend | 19 | python, go, rust, java, c#, php, rails, nestjs | database |
| testing | 18 | playwright, selenium, cucumber, unit, e2e, qa | code-quality |
| ai-ml | 17 | prompt-engineer, rag, fine-tuning, deep-research | backend, database |
| automation | 17 | planner, executor, verifier, autofix, context | all categories |
| productivity | 13 | seo, i18n, file-organizer, domain-name | utilities |
| integrations | 12 | github, shopify, wordpress, salesforce, jira | backend |
| documentation | 11 | pdf, docx, xlsx, pptx, slides, changelog | utilities |
| architecture | 10 | api-designer, microservices, cloud, mcp | backend, frontend |
| code-quality | 9 | code-review, debugger, spec-miner, the-fool | all categories |
| frontend | 9 | react, vue, angular, nextjs, typescript | backend |
| ui-ux | 5 | ui-designer, canvas, artifacts, style-picker | frontend |
| mobile | 4 | flutter, react-native, iOS, appium | backend |
| languages | 4 | clojure, shadow-cljs | devops |
| database | 2 | sql-pro, postgres-pro, database-optimizer | backend |

## Skill Count Summary

```
Total: 364 skills
Categories: 19
Largest: security (87) + workflow (52) + devops (27) = 46%
Smallest: database (2) + languages (4) + mobile (4) = 3%
```
