# Kairos — Standard Workflows

## 1. Full Feature Development
```
User Request
  → Orchestrator (parse + route)
    → Task Planner (break down)
      → Repository Analyzer (understand codebase)
        → Architecture Reviewer (verify approach)
          → Backend Engineer (implement API)
            → Frontend Engineer (implement UI)
              → Security Auditor (review)
                → Performance Optimizer (optimize)
                  → Testing Engineer (write tests)
                    → Code Reviewer (final review)
                      → Documentation Writer (document)
                        → Release Manager (ship)
                          → Verification Agent (validate)
```

## 2. Bug Fix
```
Bug Report
  → Orchestrator
    → Bug Finder (reproduce + locate)
      → Crash Analyzer (root cause)
        → Bug Fixer (implement fix)
          → Regression Tester (verify no regression)
            → Code Reviewer (review fix)
              → Release Manager (deploy)
```

## 3. Code Review
```
Pull Request
  → Orchestrator
    → Code Reviewer (general review)
      → Security Auditor (security review)
        → Performance Optimizer (performance review)
          → Architecture Reviewer (architecture review)
            → Staff Engineer Reviewer (deep review)
              → Orchestrator (merge decision)
```

## 4. Security Audit
```
Security Request
  → Orchestrator
    → Secrets Scanner (scan credentials)
      → Dependency Auditor (scan dependencies)
        → OWASP Specialist (vulnerability scan)
          → Auth Reviewer (auth review)
            → API Security Auditor (API review)
              → Supply Chain Auditor (supply chain)
                → Penetration Review Agent (pen test)
                  → Security Auditor (final report)
```

## 5. Performance Optimization
```
Performance Request
  → Orchestrator
    → Performance Regression Detector (baseline)
      → CPU Optimizer (CPU profile)
        → Memory Optimizer (memory profile)
          → Bundle Optimizer (bundle analysis)
            → Network Optimizer (network audit)
              → Database Optimizer (query audit)
                → Caching Optimizer (cache strategy)
                  → Algorithm Optimizer (algorithm review)
                    → Build Optimizer (build optimization)
```

## 6. Architecture Review
```
Architecture Request
  → Orchestrator
    → Repository Mapper (map codebase)
      → Solution Architect (design review)
        → System Architect (system review)
          → Microservices Architect (microservices)
            → Cloud Architect (cloud review)
              → Database Architect (data review)
                → Architecture Reviewer (final review)
```

## 7. Testing Campaign
```
Test Request
  → Orchestrator
    → Unit Test Engineer (unit tests)
      → Integration Test Engineer (integration)
        → E2E Test Engineer (e2e tests)
          → Coverage Analyzer (coverage report)
            → Performance Tester (load tests)
              → Accessibility Tester (a11y tests)
                → Regression Tester (regression suite)
                  → QA Engineer (final QA)
```

## 8. Documentation Generation
```
Documentation Request
  → Orchestrator
    → README Generator (readme)
      → API Documentation Writer (API docs)
        → Code Documenter (code docs)
          → Architecture Documentation Writer (architecture)
            → Changelog Generator (changelog)
              → Comment Generator (code comments)
```

## 9. Deployment Pipeline
```
Deploy Request
  → Orchestrator
    → CI/CD Engineer (pipeline check)
      → Docker Engineer (container build)
        → Kubernetes Engineer (deploy config)
          → Infrastructure Engineer (infra check)
            → Deployment Engineer (execute deploy)
              → Monitoring Engineer (verify health)
                → SRE Engineer (SLO validation)
```

## 10. Research Investigation
```
Research Request
  → Orchestrator
    → GitHub Research Agent (code research)
      → Documentation Research Agent (docs research)
        → Technology Comparison Agent (comparison)
          → Best Practice Research Agent (best practices)
            → Deep Research Agent (deep analysis)
              → Architecture Research Agent (arch research)
```

## Workflow Rules
- Each step must complete before the next begins
- If any step fails, the Orchestrator is notified
- Failed steps can be retried with additional context
- Parallel execution is allowed for independent steps
- Each step receives only the context it needs
