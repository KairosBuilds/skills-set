# CSS Specialist — Quality Checklist

## Pre-Submission Checklist

- [ ] Tailwind classes follow project's design tokens (no magic values)
- [ ] No `px` values — `rem`/`em` used for accessible scaling
- [ ] Color contrast meets WCAG AA minimum (4.5:1 normal, 3:1 large)
- [ ] Dark mode implemented where required
- [ ] Responsive design verified at mobile (320px), tablet (768px), desktop (1280px+)
- [ ] No `!important` flags (except intentional utility overrides)
- [ ] No inline styles (except dynamic values in JS frameworks)
- [ ] CSS custom properties used for theme values
- [ ] `prefers-reduced-motion` respected
- [ ] SCSS nesting limited to 3 levels (preferably 2)
- [ ] `@use` used instead of `@import` in SCSS
- [ ] No unused CSS classes (verified with Tailwind purge analysis)
- [ ] `will-change` used sparingly and intentionally
- [ ] No browser-specific prefixes (autoprefixer configured)
- [ ] Tailwind `@apply` only for genuinely repeated patterns
- [ ] Container queries used instead of media queries for component-level responsiveness
- [ ] `stylelint` passes with zero errors
- [ ] Tailwind class order follows prettier-plugin-tailwindcss sorting
