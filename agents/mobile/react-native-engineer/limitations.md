# Limitations — React Native Engineer

## Technical Limitations
1. **Native Performance**: Cannot match fully native apps for GPU-intensive tasks (AR, complex games, video processing)
2. **Platform-Specific APIs**: New iOS/Android APIs may have weeks-to-months lag before React Native wrappers are available
3. **Bundle Size**: React Native apps are typically 8-15MB larger than native equivalents
4. **Startup Time**: Hermes improves this, but cold start is 2-3x slower than native
5. **Debugging Complexity**: Native crashes require knowledge of both iOS (Xcode) and Android (Android Studio) tooling
6. **Third-Party Native Modules**: Compatibility issues when upgrading RN versions with community maintained modules
7. **Memory Management**: Less control over memory compared to native; complex animations can cause OOM on low-end devices

## Process Limitations
1. **Build Time**: Metro bundler can be slow for large projects; incremental builds help but are imperfect
2. **Code Sharing**: While cross-platform in theory, ~15-25% of code is still platform-specific
3. **New Architecture Migration**: Gradual migration to Fabric/TurboModules requires significant refactoring effort
4. **Expo Limitations**: Expo managed workflow restricts access to some native APIs; may need to eject
5. **Apple Review**: React Native apps are subject to the same App Store review process with no shortcuts

## Scope Constraints
1. **Not suitable for**: AR/VR experiences, AAA games, system-level utilities, hardware drivers
2. **Edge cases**: Background services, Bluetooth peripherals, custom keyboard extensions
3. **Complex integrations**: SIP calling, real-time audio processing, custom metal shaders
