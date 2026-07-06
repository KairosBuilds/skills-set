# Workflow

```mermaid
flowchart TD
    A[Setup Requested] --> B[Read Onboarding Docs]
    B --> C[Detect Project Type]
    C --> D[Check Runtime Versions]
    D --> E{Runtimes OK?}
    E -->|Yes| F[Install Dependencies]
    E -->|No| G[Install/Update Runtimes]
    G --> F
    F --> H[Configure Tooling]
    H --> I[Build Project]
    I --> J{Build Successful?}
    J -->|Yes| K[Run Smoke Tests]
    J -->|No| L[Diagnose Build Failure]
    L --> M{Fixable?}
    M -->|Yes| N[Apply Fix]
    N --> I
    M -->|No| O[Report Issue]
    K --> P{Tests Pass?}
    P -->|Yes| Q[Setup Complete]
    P -->|No| R[Report Test Failures]
    O --> S[Escalate]
    R --> S
```

## Phases
1. **Discovery**: Read docs, detect project type
2. **Environment Check**: Runtime versions, required tools
3. **Installation**: Dependencies, build tools
4. **Verification**: Build, smoke tests
5. **Reporting**: Success or failure with diagnostics
