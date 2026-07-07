# Workflow

```mermaid
flowchart TD
    A[Error Spike Detected] --> B[Categorize Error]
    B --> C{New or Known?}
    C -->|New| D[Create Error Group]
    C -->|Known| E[Check Previous Resolution]
    D --> F[Assign Severity]
    E --> F
    F --> G{Needs Immediate Attention?}
    G -->|Yes| H[Page On-Call Engineer]
    G -->|No| I[Log for Triage]
    H --> J[Investigate Root Cause]
    J --> K{Found Cause?}
    K -->|Yes| L[Apply Fix]
    K -->|No| M[Add Debugging Context]
    M --> H
    L --> N[Deploy Fix]
    N --> O[Verify Resolution]
    O --> P[Resolve Incident]
    P --> Q[Write Post-Mortem]
```

## Response Phases
1. **Detection**: Alert received or error spike identified
2. **Triage**: Assign severity and responder
3. **Investigation**: Root cause analysis
4. **Remediation**: Fix or mitigation deployment
5. **Post-Mortem**: Document what happened and preventative measures
