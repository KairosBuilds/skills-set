# Skill Resolver

## Purpose
Automatically determine which skills an agent requires for a given task.

## Resolution Algorithm
1. Parse task description for technology keywords
2. Match keywords against agent's supported_skills list
3. For each matched skill, check if it exists in skills/ directory
4. If skill exists → load it
5. If skill doesn't exist → report missing skill to Orchestrator
6. If multiple skills match → load the most specific one
7. Never load optional skills unless explicitly needed

## Keyword Mapping
| Keyword | Skill Category | Specific Skill |
|---------|---------------|----------------|
| react, jsx, tsx | frontend | react-expert |
| vue, vue3 | frontend | vue-expert |
| angular | frontend | angular-architect |
| next.js, nextjs | frontend | nextjs-developer |
| python, django, fastapi | backend | python-pro, django-expert, fastapi-expert |
| node, express, nest | backend | nestjs-expert, nodejs |
| golang, go | backend | golang-pro |
| rust | backend | rust-engineer |
| database, sql, nosql | database | sql-pro, postgres-pro, database-optimizer |
| docker, container | devops | docker-compose-control |
| kubernetes, k8s | devops | kubernetes-specialist |
| terraform, iac | devops | terraform-engineer |
| ci/cd, pipeline | devops | devops-engineer |
| security, vuln | security | security-reviewer |
| test, testing, jest | testing | test-master |
| api, rest, graphql | architecture | api-designer, graphql-architect |

## Usage
Agents should call this resolver during initialization to determine which skills to load for the current task.
