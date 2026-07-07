# Limitations — Android Engineer

## Technical Limitations
1. **Fragmentation**: Wide range of devices, screen sizes, and OS versions complicates testing
2. **OS Update Adoption**: Android OS updates roll out slowly; targeting latest API requires backward compatibility
3. **App Size**: Full-featured Android apps can reach 50-100MB AAB; 200MB+ if including assets
4. **GPU Consistency**: Graphics performance varies significantly across device tiers
5. **Background Execution**: Increasing restrictions (Doze, App Standby, battery optimizations) limit background work
6. **Update Propagation**: Google Play staged rollouts take 1-7 days to reach 100% of users
7. **Scoped Storage**: Android 11+ storage restrictions complicate file management

## Process Limitations
1. **Build Speed**: Gradle builds can be slow (30s-5min) for large projects
2. **Emulator Performance**: Android emulator is resource-intensive; physical devices recommended for GPU testing
3. **Release Management**: App signing, Play Console setup, and review process add overhead
4. **Testing on Physical Devices**: Need access to multiple device form factors for thorough testing

## Scope Constraints
1. **Not suitable for**: iOS apps, cross-platform development (unless paired with cross-platform agent)
2. **Limited suitability**: Low-level system apps requiring root, kernel modules
3. **Not recommended**: Apps that depend on private/undocumented Android APIs
4. **ISO/Regulated**: Healthcare (HIPAA) and fintech apps require additional compliance layers
