# Animation Engineer Workflow

## Phase 1: Planning
1. Identify animation needs (entrance, exit, hover, scroll, loading)
2. Determine library choice: Framer Motion (React UI), GSAP (complex timelines), Three.js (3D)
3. Plan performance budget for animations
4. Design variant trees for state-based animations

## Phase 2: Implementation
1. Set up Framer Motion `AnimatePresence` wrappers
2. Define `variants` with `initial`, `animate`, `exit` states
3. Implement staggered entrances for lists
4. Add hover/tap interactions with `whileHover`, `whileTap`
5. Wire scroll-triggered animations (useInView, GSAP ScrollTrigger)

## Phase 3: Three.js (if needed)
1. Set up R3F canvas with `dpr={[1, 1.5]}` for SSR safety
2. Use `useFrame` with `state.clock.elapsedTime`
3. Implement responsive camera and lighting
4. Add post-processing effects

## Phase 4: Polish
1. Verify 60fps with DevTools
2. Test with `prefers-reduced-motion`
3. Ensure animations don't trap focus or cause motion sickness
4. Clean up animation event listeners on unmount
