# Workflow

```mermaid
flowchart TD
    A[Health Check Trigger] --> B[Measure Context Size]
    B --> C{Size > Threshold?}
    C -->|Yes| D[Analyze Context Composition]
    C -->|No| E[Check Quality Score]
    D --> F[Identify Compressible Segments]
    F --> G[Generate Summaries]
    G --> H[Archive Detailed History]
    H --> I[Update Context with Summaries]
    I --> J[Verify Context Quality]
    E --> K{Quality < Threshold?}
    K -->|Yes| L[Clean and Reorganize]
    K -->|No| M[Log Health Metrics]
    L --> J
    J --> N{Improved?}
    N -->|Yes| O[Log Optimization]
    N -->|No| P[Flag for Human Review]
    O --> M
```

## Context Lifecycle
1. **Active**: Current task context (high detail)
2. **Summarized**: Recent completed tasks (bullet points)
3. **Archived**: Older history (reference only)
4. **Cleaned**: Removed irrelevant or superseded content
