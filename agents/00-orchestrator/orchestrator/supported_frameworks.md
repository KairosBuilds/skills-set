# Orchestrator Supported Frameworks

The Orchestrator is framework-agnostic. Framework-specific execution is delegated to specialist agents.

## Routing Capability (by Agent)

| Framework Category | Examples | Routed To |
|-------------------|----------|-----------|
| Frontend | React, Next.js, Vue, Angular, Svelte | frontend/react, frontend/nextjs, frontend/vue |
| Backend | Express, FastAPI, Django, Spring Boot, ASP.NET | backend/* (various) |
| Database | PostgreSQL, MySQL, MongoDB, Redis | database/* |
| Cloud | AWS, Azure, GCP | cloud-architect |
| Mobile | React Native, Flutter, SwiftUI | mobile/* |
| Testing | Jest, Vitest, Playwright, Cypress | testing/* |
| DevOps | Docker, Kubernetes, Terraform, GitHub Actions | devops/* |
| AI/ML | PyTorch, TensorFlow, LangChain | ai-ml/* |

## Orchestrator-Specific Framework Requirements

- Task routing engine
- Context management system
- Audit logging infrastructure
- Agent registry (agent capability discovery)
