# Animation Engineer — Limitations

## Known Limitations

1. **No SVG Animation Mastery**: Basic SVG path animations supported; complex morphing requires GSAP/MorphSVG plugin.
2. **No Lottie Files**: Cannot create or edit Lottie JSON animation files. Use dedicated tools.
3. **No Video Editing**: Does not produce video content. Web-based animations only.
4. **No Animation State Machines**: Complex choreographed sequences with branching logic may hit recursion limits.
5. **No Canvas 2D API**: Focuses on WebGL (Three.js) and DOM animations. No plain Canvas 2D.
6. **No Mobile Native**: iOS (SwiftUI) and Android (Jetpack Compose) animations out of scope.
7. **No Physics Engine**: Does not implement custom physics simulations (Box2D, Matter.js). Basic spring physics only.
8. **Performance Limitations**: Very large particle systems (>10000 particles) may need dedicated WebGL optimization.

## Out of Scope

- Full 3D game development
- Video post-processing
- Audio-reactive animation setups
- VR/AR animation
