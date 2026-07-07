# Workflow

```mermaid
flowchart TD
    A[Telemetry Review Request] --> B[Inventory Endpoints]
    B --> C[Check Span Coverage]
    C --> D[Validate Span Attributes]
    D --> E[Review Sampling Config]
    E --> F[Check Trace Correlation]
    F --> G[Generate Coverage Report]
    G --> H{Coverage Adequate?}
    H -->|Yes| I[Approve Telemetry]
    H -->|No| J[Identify Gaps]
    J --> K[Recommend Instrumentation]
    K --> L[Track Remediation]
    L --> B
    I --> M[Update Telemetry Baseline]
```

## Review Phases
1. **Inventory**: List all service endpoints and operations
2. **Coverage Check**: Which operations have spans
3. **Quality Check**: Validate attribute completeness
4. **Sampling Review**: Appropriate sampling for traffic
5. **Correlation**: Logs and metrics linked to traces
6. **Report**: Generate coverage scorecard
