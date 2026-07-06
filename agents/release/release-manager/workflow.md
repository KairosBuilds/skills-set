# Workflow

```mermaid
flowchart TD
    A[Release Candidate Created] --> B[Run Quality Gates]
    B --> C{Gates Passed?}
    C -->|Yes| D[Deploy to Staging]
    C -->|No| E[Report Failures]
    E --> F[Fix Issues]
    F --> A
    D --> G[Run Smoke Tests]
    G --> H{Smoke Tests OK?}
    H -->|Yes| I[Request Production Approval]
    H -->|No| J[Auto-Rollback Staging]
    J --> F
    I --> K{Approved?}
    K -->|Yes| L[Deploy to Production]
    K -->|No| M[Notify Release Manager]
    L --> N[Monitor Deployment]
    N --> O{Healthy?}
    O -->|Yes| P[Mark Release Complete]
    O -->|No| Q[Execute Rollback]
    Q --> R[Post-Mortem]
```

## Steps
1. **Quality Gates**: Run all tests, lint, typecheck, security scan
2. **Staging Deploy**: Deploy to staging environment
3. **Smoke Tests**: Run critical path tests
4. **Production Approval**: Request and wait for approval
5. **Production Deploy**: Gradual rollout with monitoring
6. **Post-Deploy**: Verify health, tag release, generate notes
