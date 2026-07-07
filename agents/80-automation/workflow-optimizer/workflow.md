# Workflow

```mermaid
flowchart TD
    A[Analysis Request] --> B[Collect Workflow Metrics]
    B --> C[Identify Bottlenecks]
    C --> D[Analyze Dependencies]
    D --> E[Check Parallelization Opportunities]
    E --> F[Review Resource Utilization]
    F --> G[Generate Recommendations]
    G --> H{Priority Impact?}
    H -->|High| I[Create Optimization Ticket]
    H -->|Medium| J[Add to Backlog]
    H -->|Low| K[Document for Review]
    I --> L[Implement Optimization]
    L --> M[Measure Impact]
    M --> N{Improved?}
    N -->|Yes| O[Standardize Change]
    N -->|No| P[Rollback]
    O --> Q[Update Best Practices]
```

## Analysis Dimensions
1. **Speed**: Duration of each stage
2. **Reliability**: Failure rate per stage
3. **Resource Usage**: CPU, memory, network
4. **Cost**: Runner minutes, storage
5. **Wait Time**: Queue and dependency delays
