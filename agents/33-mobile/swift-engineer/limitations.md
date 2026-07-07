# Limitations — Swift Engineer

## Technical Limitations
1. **Linux Support**: Swift on Linux has fewer system framework equivalents (no Core Data, no SwiftUI)
2. **Windows Support**: Swift on Windows is experimental; not production-ready for most use cases
3. **Server Ecosystem**: Swift server-side ecosystem is smaller than Node.js, Python, or Java
4. **Concurrency Maturity**: Swift structured concurrency (5.5+) still has edge cases with legacy codebases
5. **SPM Limitations**: Package plugins are less mature than Gradle or npm equivalents
6. **Binary Size**: Swift static linking produces larger binaries than equivalent C/C++ or Go
7. **Runtime Compatibility**: Swift runtime version must match across linked libraries

## Process Limitations
1. **Build Speed**: Swift compilation is slower than interpreted languages; incremental builds help
2. **Linux CI**: Requires Docker or Linux runner for cross-platform testing
3. **Resource Availability**: Fewer Swift-specific libraries and tools compared to other languages
4. **Hiring**: Smaller talent pool for server-side Swift compared to Node.js or Python
5. **Tooling Maturity**: Some IDE features (refactoring, code generation) are less mature for Swift

## Scope Constraints
1. **Not suitable for**: Android development, embedded systems, front-end web (use WASM experiments only)
2. **Limited suitability**: Real-time audio processing, game development (use Metal directly)
3. **Not recommended**: Apps exclusively targeting Linux without macOS development team
4. **Newer domain**: Server-side Swift is still gaining ecosystem maturity
