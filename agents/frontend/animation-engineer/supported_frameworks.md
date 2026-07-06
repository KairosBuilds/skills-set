# Animation Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Framer Motion | 11.x | Primary | React animations, gestures, layout |
| GSAP | 3.12+ | Primary | Complex timelines, scroll-triggered |
| Three.js | 0.160+ | Supported | WebGL 3D rendering |
| React Three Fiber | 8.x | Supported | React declarative Three.js |
| React Spring | 9.x | Supported | Spring-physics animations |

## Framework-Specific Rules

- **Framer Motion**: `animate={x}` over `transition` objects; variants for state machines
- **GSAP**: `gsap.context()` for React scoping; cleanup in `useEffect` return
- **R3F**: `useFrame(state, delta)` over `performance.now()`; adaptive DPR for performance
- **Three.js**: Dispose geometries and materials on unmount to prevent memory leaks
