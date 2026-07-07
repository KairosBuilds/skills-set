# Execution Rules for Responsive Design Engineer Agent

## Core Rules

1. **Mobile-First**: Build for mobile screens first, then enhance for larger screens using `min-width` media queries.
2. **CSS Grid for Layout**: Use CSS Grid for page-level and section-level layouts. Use Flexbox for component-level alignment.
3. **Container Queries**: Use `@container` queries for component-level responsiveness instead of viewport media queries for reusable components.
4. **Fluid Typography**: Use `clamp()` for font sizes. Never use fixed pixel sizes for text.
5. **Fluid Spacing**: Use relative units (`rem`, `vw`, `clamp`) for margins and padding.
6. **Breakpoint Strategy**: Use Tailwind defaults (`sm: 640px`, `md: 768px`, `lg: 1024px`, `xl: 1280px`). Add custom breakpoints only when data shows user behavior changes.
7. **Images**: Use responsive images with `srcset` and `sizes`. Use `max-width: 100%` and `height: auto`.
8. **Touch Targets**: Minimum 44x44px touch targets on mobile. Adequate spacing between interactive elements.
9. **Content Priority**: Critical content first on mobile. Progressive enhancement with screen size.
10. **Testing**: Test on real devices, not just DevTools responsive mode.

## Prohibited

- Fixed-width containers (use `max-width` with responsive padding)
- Horizontal overflow (no fixed-width elements that exceed viewport)
- `px` for font sizes (use `rem`, `clamp`)
- Hover-only interactions without tap alternatives
- Tables without horizontal scroll wrapper on mobile
- `min-device-width` (use `min-width` for accurate media queries)
- Overflow hidden on body (breaks layout)

## Enforcement

Test with Chrome DevTools device emulation at 320px, 768px, 1024px, 1440px.
