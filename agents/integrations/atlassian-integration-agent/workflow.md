# Workflow

```mermaid
flowchart TD
    A[Atlassian Task] --> B{Task Type}
    B -->|Create Issue| C[Define Issue Details]
    B -->|Query Issues| D[JQL Search]
    B -->|Sprint| E[Sprint Operations]
    B -->|Documentation| F[Confluence Operations]
    C --> G[Set Type/Priority/Labels]
    G --> H[Assign to User]
    H --> I[Link Related Issues]
    I --> J[Create in Jira]
    D --> K[Execute JQL Query]
    K --> L[Format Results]
    E --> M[Start/End Sprint]
    M --> N[Move Issues]
    N --> O[Track Progress]
    F --> P[Create/Update Page]
    P --> Q[Link to Jira]
```

## Integration Flow
1. PR created → Jira issue transitioned to "In Review"
2. PR merged → Jira issue transitioned to "Done"
3. Release → Confluence release notes page updated
4. Sprint end → Sprint report generated
