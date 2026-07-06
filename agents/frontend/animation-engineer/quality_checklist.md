# Animation Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] Animations maintain 60fps (verified with Chrome DevTools)
- [ ] Only `transform` and `opacity` animated for GPU compositing
- [ ] `will-change` set on animated elements
- [ ] `prefers-reduced-motion` respected with non-animated fallback
- [ ] Framer Motion spring physics used (stiffness 300-400, damping 25-30)
- [ ] No layout-triggering properties animated (width, height, margin)
- [ ] `AnimatePresence` used for mount/unmount transitions
- [ ] `layoutId` used for shared element transitions
- [ ] Stagger children values are 0.04-0.08 with delayChildren
- [ ] Three.js scenes lazy-loaded with dynamic import
- [ ] R3F `useFrame` uses `state.clock.elapsedTime` not `performance.now()`
- [ ] Three.js geometries and materials disposed on unmount
- [ ] GSAP `gsap.context()` scoped and cleaned up
- [ ] No animation frame leaks (requestAnimationFrame cancelled on unmount)
- [ ] Hover/tap animations have `whileHover`/`whileTap` where appropriate
- [ ] Scroll-linked animations use `useInView` with `once: true`
- [ ] No motion sickness triggers (large parallax, rapid scaling)
- [ ] Animation event handlers cleaned up
- [ ] dark mode respected for animation visibility
