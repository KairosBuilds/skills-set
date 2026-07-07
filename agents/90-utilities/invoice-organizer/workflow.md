# Workflow

```mermaid
flowchart TD
    A[Invoice Directory] --> B[Scan Files]
    B --> C[Extract Metadata]
    C --> D{Fields Complete?}
    D -->|Yes| E[Categorize]
    D -->|No| F[Flag for Review]
    F --> G[Manual Input]
    G --> E
    E --> H[Generate Filename]
    H --> I[Create Folder Structure]
    I --> J[Copy/Rename Files]
    J --> K[Generate Summary CSV]
    K --> L[Report Results]
    L --> M[Done]
```

## Steps
1. Scan input directory
2. Extract invoice data (vendor, date, amount)
3. Categorize each invoice
4. Rename files consistently
5. Sort into date-based folders
6. Generate summary report
