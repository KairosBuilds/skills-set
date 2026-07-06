# Execution Rules for Accessibility Engineer Agent

## Core Rules

1. **Semantic HTML First**: Use native HTML elements (`<button>`, `<nav>`, `<main>`, `<header>`, `<footer>`) before ARIA. ARIA only when semantic HTML is insufficient.
2. **WCAG 2.2 AA Minimum**: All work must meet WCAG 2.2 Level AA. AAA where specified.
3. **Keyboard Navigation**: All interactive elements must be keyboard accessible. Visible focus indicators required (minimum 2:1 contrast ratio against unfocused state).
4. **ARIA Patterns**: Follow WAI-ARIA Authoring Practices for complex widgets (tabs, modals, accordions, carousels, tree views).
5. **Color Contrast**: Minimum 4.5:1 for normal text, 3:1 for large text (18px+ bold or 24px+ regular). Non-text elements need 3:1 contrast.
6. **Screen Reader Labels**: All interactive elements have accessible names. Images have meaningful `alt` text. Icons have `aria-label` or visually hidden text.
7. **Focus Management**: Trap focus in modals and sidebars. Return focus on close. Manage tab order with logical DOM order.
8. **Live Regions**: Use `aria-live` regions for dynamic content updates (toast messages, loading states, search results).
9. **Error Identification**: Form errors must be programmatically associated with inputs. Error messages in `aria-describedby`.
10. **Reduced Motion**: Respect `prefers-reduced-motion`. Provide alternative static experience.

## Prohibited

- `<div>` as interactive element without proper ARIA
- `role="button"` on `<div>`/`<span>` (use `<button>`)
- `aria-hidden="true"` on focusable elements
- `tabindex` > 0 (use logical DOM order)
- Auto-playing media without pause/stop controls
- Mouse-only event handlers (add keyboard equivalents)
- Disabling zoom (`user-scalable=no`, `maximum-scale=1.0`)
- Colour as sole indicator of state or information

## Enforcement

Run axe DevTools, Lighthouse accessibility audit, and manual keyboard navigation test.
