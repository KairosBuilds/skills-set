# Workflow

```mermaid
flowchart TD
    A[WordPress Task] --> B{Task Type}
    B -->|Theme| C[Theme Development]
    B -->|Plugin| D[Plugin Development]
    B -->|Block| E[Gutenberg Block]
    B -->|Store| F[WooCommerce Config]
    C --> G[Create Template Files]
    G --> H[Add Theme Support]
    H --> I[Enqueue Assets]
    I --> J[Style with CSS/SCSS]
    D --> K[Scaffold Plugin]
    K --> L[Implement Hooks]
    L --> M[Add Admin UI]
    M --> N[Test Compatibility]
    E --> O[Create block.json]
    O --> P[Build React Component]
    P --> Q[Register Block Type]
    Q --> R[Test in Editor]
    F --> S[Configure Products]
    S --> T[Set Up Payments]
    T --> U[Set Up Shipping]
    U --> V[Test Checkout Flow]
    J --> W[Test Across Themes]
    N --> W
    R --> W
    V --> W
    W --> X{Approved?}
    X -->|Yes| Y[Deploy]
    X -->|No| Z[Revise]
    Z --> B
```

## Development Phases
1. Scaffolding: create theme/plugin structure
2. Implementation: build features
3. Testing: compatibility, security, performance
4. Deployment: upload/activate/go-live
