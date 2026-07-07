# Execution Rules for CSS Specialist Agent

## Core Rules

1. **Tailwind First**: Use Tailwind utility classes over custom CSS. Extract repeated patterns into components, not custom CSS classes.
2. **Design Tokens**: Use CSS custom properties for design tokens. Configure `tailwind.config.js` with project's design system values.
3. **Responsive by Default**: Build mobile-first. Use Tailwind breakpoints (`sm:`, `md:`, `lg:`, `xl:`).
4. **Performance**: Avoid expensive properties (`box-shadow` on animation, `filter` on large areas). Use `will-change` sparingly.
5. **SCSS Organization**: Use partials, variables, mixins. Nesting limited to 3 levels max.
6. **CSS Modules**: Scoped styles by default. Use composition over inheritance.
7. **Accessibility**: Ensure color contrast ratios (WCAG AA minimum). Support `prefers-reduced-motion`, `prefers-color-scheme`.
8. **Browser Support**: Use `@supports` for progressive enhancement. Layer fallbacks for older browsers.
9. **Spacing**: Use consistent spacing scale. Configure custom spacing in Tailwind config.
10. **Dark Mode**: Implement using `class` strategy with Tailwind dark mode. Use CSS custom properties for complex color schemes.

## Prohibited

- `!important` (except for utility overrides in specific cases)
- Inline styles (except for dynamic values in JS frameworks)
- ID selectors for styling
- `px` values (use `rem`/`em` for accessible scaling)
- Deep nesting (>4 levels in SCSS)
- `@import` (use `@use` in SCSS)
- Browser-specific prefixes (autoprefixer handles these)

## Enforcement

Verify with Tailwind compiler, check for unused classes with Tailwind's built-in purge.
