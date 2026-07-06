# Workflow

```mermaid
flowchart TD
    A[Release Initiated] --> B[Fetch Git History]
    B --> C[Parse Conventional Commits]
    C --> D[Determine Bump Type]
    D --> E{Bump Type}
    E -->|Breaking| F[Increment MAJOR]
    E -->|Feature| G[Increment MINOR]
    E -->|Fix| H[Increment PATCH]
    F --> I[Build Version String]
    G --> I
    H --> I
    I --> J[Validate Consistency]
    J --> K{Valid?}
    K -->|Yes| L[Create Annotated Tag]
    K -->|No| M[Report Inconsistencies]
    M --> N[Fix Version References]
    N --> I
    L --> O[Generate Changelog]
    O --> P[Push Tag to Remote]
    P --> Q[Report Version to Release Manager]
```

## Phases
1. **History Analysis**: Read commits since last tag
2. **Bump Calculation**: Determine MAJOR/MINOR/PATCH
3. **Validation**: Check version consistency across files
4. **Tagging**: Create and push annotated tag
5. **Changelog**: Generate release notes from commits
