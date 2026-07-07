# Execution Rules for UI Polish Agent

## Core Rules

1. **Micro-Interactions**: Every interactive element needs hover, active, and transition states. Use Tailwind `transition-all` or Framer Motion `whileHover`/`whileTap`.
2. **Glassmorphism**: Use `backdrop-blur-xl`, `bg-white/10` (or dark variant), `border border-white/20`, `shadow-xl` for glass effects. Ensure text remains readable with sufficient contrast.
3. **Neon/Lighting Effects**: Use `box-shadow` with theme color glow (`shadow-[0_0_20px_rgba(var(--color-primary),0.5)]`). Combine with `text-shadow` for text glow.
4. **Elevation**: Use consistent shadow scale. Cards should lift on hover with `transition-shadow` and `hover:shadow-lg`/`hover:shadow-xl`.
5. **Borders and Radius**: Consistent `border-radius` scale (tailwind: `rounded-sm`, `rounded-md`, `rounded-lg`, `rounded-xl`, `rounded-2xl`).
6. **Gradients**: Use Tailwind gradient utilities (`bg-gradient-to-br from-purple-500 to-blue-600`). Keep gradients subtle and purposeful.
7. **Spacing Rhythm**: Review and fix inconsistent spacing. All spacing should follow the 4px/8px grid system.
8. **Typography Polish**: Check `line-height` (leading), `letter-spacing` (tracking), font weight consistency. Add `text-balance` for headings.
9. **Dark Mode**: Every visual effect must have a dark mode counterpart. Test all polish in both themes.
10. **Consistency**: Apply same visual patterns across similar components. If cards have hover lift, all cards should have hover lift.

## Prohibited

- Visual effects that harm performance (excessive blur, multiple shadows on animated elements)
- Inconsistent border-radius across similar components
- Missing hover/focus states on interactive elements
- Unreadable glass effects (too much blur + low opacity)
- Clashing gradients
- Overly aggressive animations that cause motion sickness
- Uneven shadows (shadows that don't match elevation hierarchy)

## Enforcement

Review visual consistency across all similar component instances. Verify both light and dark modes.
