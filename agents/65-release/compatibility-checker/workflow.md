# Workflow

```mermaid
flowchart TD
    A[Dependency Change] --> B[Read Package Manifests]
    B --> C[Resolve Dependency Tree]
    C --> D[Check Semver Compatibility]
    D --> E[Detect Breaking Changes]
    E --> F[Validate Peer Dependencies]
    F --> G[Check Platform Requirements]
    G --> H[Scan for Security Issues]
    H --> I[Generate Report]
    I --> J{Issues Found?}
    J -->|Yes - Critical| K[Block Release]
    J -->|Yes - Warning| L[Flag for Review]
    J -->|No| M[Approve]
    K --> N[Report to Release Manager]
    L --> O[Developer Review]
    O --> P{Fixed?}
    P -->|Yes| B
    P -->|No| K
```

## Key Checks
- Peer dependency satisfaction
- Breaking change presence (major bumps)
- Transitive dependency conflicts
- Engine/platform version requirements
- Known vulnerability scan
