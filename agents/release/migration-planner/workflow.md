# Workflow

```mermaid
flowchart TD
    A[Migration Required] --> B[Assess Impact]
    B --> C{Type?}
    C -->|Schema| D[Generate SQL Scripts]
    C -->|Data| E[Write Data Transformation]
    C -->|Platform| F[Design Strangler Fig]
    D --> G[Generate Rollback]
    E --> G
    F --> G
    G --> H[Review with Team]
    H --> I[Test on Staging]
    I --> J{Tests Pass?}
    J -->|Yes| K[Schedule Migration Window]
    J -->|No| L[Fix Issues]
    L --> D
    K --> M[Execute Migration]
    M --> N{Successful?}
    N -->|Yes| O[Verify Integrity]
    N -->|No| P[Execute Rollback]
    P --> Q[Investigate Failure]
    O --> R[Update Documentation]
```

## Phases
1. **Assessment**: Impact analysis, risk evaluation, dependency check
2. **Scripting**: Generate migration and rollback scripts
3. **Validation**: Test on staging, verify integrity
4. **Execution**: Run during scheduled window with monitoring
5. **Verification**: Post-migration data integrity checks
