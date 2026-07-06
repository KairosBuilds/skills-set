# Accessibility Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] Semantic HTML elements used over `<div>` + ARIA
- [ ] All interactive elements keyboard accessible (Tab, Enter, Escape, Arrow keys)
- [ ] Visible focus indicators on all interactive elements (minimum 2:1 contrast)
- [ ] `aria-label` or accessible name on all interactive elements
- [ ] Images have meaningful `alt` text (decorative images have `alt=""`)
- [ ] Form inputs have associated `<label>` elements
- [ ] Form errors programmatically linked via `aria-describedby`
- [ ] `aria-live` regions for dynamic content updates
- [ ] Modal/flyout focus trapped and restored on close
- [ ] `prefers-reduced-motion` respected
- [ ] Color is not the sole indicator of state (add icon or text)
- [ ] Text contrast meets WCAG AA (4.5:1 normal, 3:1 large)
- [ ] Non-text contrast meets 3:1 (icons, focus indicators, input borders)
- [ ] No `aria-hidden="true"` on focusable elements
- [ ] `tabindex` > 0 not used (logical tab order)
- [ ] Heading hierarchy is logical (h1 → h2 → h3, no skips)
- [ ] Landmarks used (`<main>`, `<nav>`, `<header>`, `<footer>`, `<aside>`)
- [ ] Links have discernible text (no "click here", "read more" without context)
- [ ] Auto-playing media has pause/stop controls
- [ ] Zoom not disabled (`user-scalable=no` not used)
- [ ] axe DevTools scan passes with zero critical/serious violations
- [ ] Lighthouse a11y score is 95+
- [ ] Screen reader navigation test completed
- [ ] Full keyboard-only navigation test completed
