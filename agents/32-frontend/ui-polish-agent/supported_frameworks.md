# UI Polish Agent — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Tailwind CSS | 3.4+ | Primary | All visual effects |
| Framer Motion | 11.x | Primary | Micro-interactions and transitions |
| styled-components | 6.x | Supported | CSS-in-JS polish |

## Framework-Specific Rules

- **Tailwind**: Configure custom shadows, blurs, and gradients in `tailwind.config.js` `theme.extend`
- **Framer Motion**: Spring transitions for natural feel; `whileHover`/`whileTap` for interactions
- **Styled Components**: Co-locate polish styles; use transient props for conditional effects
