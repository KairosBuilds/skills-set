# Responsive Design Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] Mobile-first approach verified (base styles, then enhancement)
- [ ] No horizontal scroll at any breakpoint (320px through 1440px)
- [ ] All content visible and readable at 320px
- [ ] Touch targets at least 44x44px on mobile
- [ ] Adequate spacing between touch targets (>8px)
- [ ] CSS Grid for layouts, Flexbox for component alignment
- [ ] Container queries used for reusable components
- [ ] Fluid typography with `clamp()` — no fixed `px` font sizes
- [ ] Fluid spacing with `rem` or `clamp()` — no `px` margin/padding
- [ ] Responsive images with `srcset`/`sizes` attributes
- [ ] Navigation works on mobile (hamburger or alternative)
- [ ] Tables have horizontal scroll wrapper on small screens
- [ ] Forms usable on mobile (proper input sizing, no zoom disable)
- [ ] Text doesn't overflow containers at any breakpoint
- [ ] No hover-only interactions (tap/click alternatives provided)
- [ ] Breakpoints match Tailwind defaults consistently
- [ ] Z-index stacking doesn't break at any viewport
- [ ] Visual elements don't overlap at breakpoint transitions
- [ ] Verified on at least one real mobile device (not just DevTools)
