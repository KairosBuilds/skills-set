# Limitations — Kotlin Mobile Engineer

## Technical Limitations
1. **iOS UI**: Compose Multiplatform for iOS is still maturing; native SwiftUI may be preferred for complex UI
2. **KMP Maturity**: KMP is stable but some libraries lack Multiplatform support
3. **Framework Size**: KMP adds ~5-10MB to app size compared to pure native
4. **Swift Interop**: Kotlin/Native to Swift interop has edge cases with optionals, collections, and closures
5. **Debugging**: Cross-platform debugging is harder — need both Android and Xcode tooling
6. **Third-Party Libraries**: Not all popular libraries have KMP versions; may need expect/actual wrappers
7. **Gradle Build Times**: KMP projects have longer Gradle configuration times

## Process Limitations
1. **Tooling Fragmentation**: Development spans Android Studio and Xcode
2. **CI Complexity**: Need runners for both Android (Linux) and iOS (macOS) builds
3. **Learning Curve**: KMP requires understanding both Android and iOS ecosystems
4. **Team Expertise**: Requires team members proficient in Kotlin + at least one mobile platform
5. **Library Updates**: Cross-platform library versions must be carefully aligned

## Scope Constraints
1. **Not suitable for**: Apps requiring extensive platform-specific UI per platform (use native agents)
2. **Limited suitability**: GPU-intensive apps, advanced camera processing
3. **Not recommended**: Apps where iOS and Android UIs diverge significantly in design
4. **Edge cases**: Platform features added in latest OS versions may have KMP integration lag
