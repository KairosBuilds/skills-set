# CSS Specialist — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Tailwind CSS | 3.4+ | Primary | Utility-first CSS framework |
| Bootstrap | 5.3+ | Supported | Utility classes and components |
| styled-components | 6.x | Supported | CSS-in-JS for React |
| Emotion | 11.x | Supported | CSS-in-JS with performance focus |
| Sass/SCSS | 1.77+ | Supported | CSS preprocessor |

## Framework-Specific Rules

- **Tailwind**: Configure design tokens in theme.extend; purge unused classes; use `@apply` for shared component styles only
- **Bootstrap**: Use utility classes over Sass customization; rely on CSS variables for theming
- **Styled Components**: Co-locate styles with components; use transient props (`$prop`) to avoid passing to DOM
