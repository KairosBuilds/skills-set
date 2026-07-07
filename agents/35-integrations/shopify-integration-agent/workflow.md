# Workflow

```mermaid
flowchart TD
    A[Shopify Task] --> B{Task Type}
    B -->|Theme| C[Theme Development]
    B -->|App| D[App Development]
    B -->|Storefront| E[Storefront Integration]
    C --> F[Create/Edit Sections]
    F --> G[Style with CSS/SCSS]
    G --> H[Add JS Interactivity]
    H --> I[Test in Preview]
    D --> J[Scaffold App]
    J --> K[Implement API Calls]
    K --> L[Set Up Webhooks]
    L --> M[Test App]
    E --> N[Set Up Hydrogen]
    N --> O[Build Storefront]
    O --> P[Integrate Cart/Checkout]
    P --> Q[Deploy]
    I --> R{Approved?}
    M --> R
    Q --> R
    R -->|Yes| S[Publish]
    R -->|No| T[Revise]
    T --> C
```

## Development Phases
1. Planning: requirements, design, data model
2. Development: theme/app/storefront code
3. Testing: preview, cross-browser, e2e
4. Deployment: publish theme, deploy app
5. Monitoring: performance, errors, sales impact
