# UI Polish Agent — Quality Checklist

## Pre-Submission Checklist

- [ ] All interactive elements have hover and active states
- [ ] Buttons have scale press effect (`active:scale-95` or similar)
- [ ] Cards have hover lift with shadow transition
- [ ] Links have underline animation or color transition on hover
- [ ] Transitions use `transition-all` or specific properties (duration 150-300ms)
- [ ] Glassmorphism effects maintain readability (not too transparent/burred)
- [ ] Shadows follow consistent elevation scale
- [ ] Border-radius is consistent across similar components
- [ ] Spacing follows 4px/8px grid system (no 7px, 13px, etc.)
- [ ] Font sizes and weights consistent across headings and body text
- [ ] Line-height (`leading`) values are consistent per text level
- [ ] Gradients use cohesive color stops
- [ ] Dark mode has equivalent polish (no dark mode blind spots)
- [ ] Neon/glow effects have proper color contrast
- [ ] No clashing visual styles (components of same type look consistent)
- [ ] Loading skeletons or spinners are styled to match the theme
- [ ] Page transitions are smooth (no flash of unstyled content)
- [ ] Skeleton loading matches the final content shape
- [ ] No visual regressions after polish (verified with comparison)
- [ ] All polish effects respect `prefers-reduced-motion`
