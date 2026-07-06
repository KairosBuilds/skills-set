# Limitations — Flutter Engineer

## Technical Limitations
1. **App Size**: Flutter release builds are 5-12MB base, plus platform-specific embedding
2. **Platform Parity**: Web and desktop support are stable but less mature than mobile targets
3. **Native API Gaps**: Some platform APIs require custom plugin development (MethodChannel)
4. **Rendering Engine**: Skia-based rendering can differ visually from native platform controls
5. **Memory Profiles**: Flutter apps use ~40-80MB baseline, higher than native equivalents
6. **Camera Preview**: Real-time camera processing is less performant than native SDKs
7. **Metal/OpenGL**: Direct GPU access requires engine-level plugins

## Process Limitations
1. **Code Generation**: build_runner slow for large projects; incremental builds improve but not perfect
2. **Hot Reload Limitations**: State loss on hot reload; some widget changes require full restart
3. **Platform Channel Overhead**: Frequent native calls via MethodChannel add latency
4. **Debug Build Performance**: Debug mode JIT is significantly slower than release AOT
5. **iOS Compilation**: First iOS build requires full compilation (slow on M-series Macs too)

## Scope Constraints
1. **Not suitable for**: System-level apps, kernel extensions, hardware driver UIs
2. **Limited suitability**: 3D gaming (use Flame or Unity instead), heavy computation apps
3. **Not recommended**: Apps requiring extensive platform-specific UI that fights platform conventions
