# Workflow

```mermaid
flowchart TD
    A[Download Request] --> B[Parse URL]
    B --> C[Check Platform Support]
    C --> D{Supported?}
    D -->|Yes| E[Get Video Info]
    D -->|No| F[Report Unsupported]
    E --> G[Select Quality/Format]
    G --> H[Start Download]
    H --> I[Show Progress]
    I --> J{Complete?}
    J -->|Yes| K[Post-Process]
    J -->|No| L[Handle Error]
    L --> M{Retry?}
    M -->|Yes| H
    M -->|No| N[Report Failure]
    K --> O{Audio Extract?}
    O -->|Yes| P[Extract Audio]
    O -->|No| Q[Save Video]
    P --> Q
    Q --> R[Verify File]
    R --> S[Report Complete]
```

## Process
1. URL validation and platform detection
2. Video information retrieval
3. Quality/format selection
4. Download with progress tracking
5. Post-processing (conversion, extraction)
6. File verification
