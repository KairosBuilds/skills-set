# Accessibility Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| WAI-ARIA | 1.2 | Primary | ARIA Authoring Practices |
| axe-core | 4.x | Primary | Automated accessibility testing |
| Lighthouse | Latest | Supported | Built-in a11y auditing |
| React Aria Components | 1.x | Supported | Accessible React components |
| Reach UI | Latest | Supported | Accessible React primitives |
| Headless UI | Latest | Supported | Unstyled accessible components |

## Framework-Specific Rules

- **axe-core**: Run with `@axe-core/playwright` for E2E a11y; configure to WCAG 2.2 AA
- **React Aria**: Use over custom ARIA when possible; follows WAI-ARIA patterns by default
- **Lighthouse**: Check a11y score; use as baseline, not sole verification
- **Headless UI**: Provides built-in keyboard navigation and ARIA attributes
