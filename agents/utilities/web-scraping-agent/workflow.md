# Workflow

```mermaid
flowchart TD
    A[Scrape Request] --> B[Parse URL]
    B --> C[Check robots.txt]
    C --> D{Allowed?}
    D -->|Yes| E[Send Request]
    D -->|No| F[Report Blocked]
    E --> G{Need JS Render?}
    G -->|Yes| H[Browser Render]
    G -->|No| I[Parse HTML]
    H --> I
    I --> J[Extract Content]
    J --> K[Clean HTML]
    K --> L[Convert to Markdown]
    L --> M{Need More Pages?}
    M -->|Yes| N[Follow Links]
    N --> E
    M -->|No| O[Structure Output]
    O --> P{Valid?}
    P -->|Yes| Q[Return Result]
    P -->|No| R[Adjust Selectors]
    R --> I
```

## Process
1. Validation: check URL, robots.txt
2. Request: fetch page content
3. Rendering: JS execution if needed
4. Extraction: parse and clean content
5. Conversion: HTML to markdown/structured data
6. Pagination: follow links if needed
