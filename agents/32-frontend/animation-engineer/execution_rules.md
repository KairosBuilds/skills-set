# Execution Rules for Animation Engineer Agent

## Core Rules

1. **60fps Target**: All animations must maintain 60fps. Use `will-change` for GPU-accelerated properties (`transform`, `opacity`).
2. **Spring Physics**: Default to spring animations (`type: 'spring'`) with stiffness 300-400, damping 25-30. Avoid duration-based timing except for simple opacity fades.
3. **Framer Motion First**: Use Framer Motion for React/Next.js projects. GSAP for non-React or complex timeline-based sequences. Three.js for 3D.
4. **Reduced Motion**: Always respect `prefers-reduced-motion`. Provide non-animated fallbacks. Use `useReducedMotion` hook in Framer Motion.
5. **Staggered Entrances**: Use `staggerChildren: 0.04-0.08` with `delayChildren` for list animations. Avoid staggering more than 20 items.
6. **AnimatePresence**: Use `AnimatePresence` for mount/unmount animations. Define `exit` variants for elements leaving the DOM.
7. **Layout Animations**: Use Framer Motion's `layout` prop for smooth reorder and resize animations. Use `layoutId` for shared element transitions.
8. **Lazy Loading**: Three.js scenes must be lazy-loaded with dynamic import. Never include Three.js in the main bundle.
9. **GPU Compositing**: Animate only `transform` and `opacity` when possible. Avoid animating `width`, `height`, `top`, `left` which trigger layout recalculations.
10. **Accessibility**: Pause animations on `:hover` and `:focus` for users who need it. Provide `pause` button for auto-playing animations.

## Prohibited

- `performance.now()` in animation frames (use `state.clock.elapsedTime` in R3F)
- `requestAnimationFrame` without cleanup on unmount
- Animations on elements that affect layout (width, height, margin)
- jQuery animations
- CSS `@keyframes` for complex state-based animations (use Framer Motion variants)
- Unthrottled scroll-based animations

## Enforcement

Verify animation performance with Chrome DevTools Performance tab. Check for layout thrashing.
