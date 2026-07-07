# Limitations — iOS Engineer

## Technical Limitations
1. **Platform Exclusivity**: Development requires macOS; cannot build iOS apps on Windows/Linux
2. **Apple Ecosystem Lock-in**: SwiftUI features require latest OS versions; adoption lag for enterprise users
3. **App Store Review**: All apps subject to App Store review (2-7 days); rejection requires resubmission cycle
4. **Closed Source**: iOS kernel and most system frameworks are closed source
5. **Memory Pressure**: iOS aggressively terminates background processes; must use BGTaskScheduler
6. **SwiftUI Limitations**: Complex custom UI still requires UIViewRepresentable bridges to UIKit
7. **Simulator Limitations**: Camera, sensors, and some hardware features unavailable in simulator

## Process Limitations
1. **Xcode Stability**: Xcode can be resource-intensive and occasionally unstable with large projects
2. **Build Time**: Swift compilation for large projects can be slow; monolithic builds benefit from module optimization
3. **CI Costs**: macOS CI runners are more expensive than Linux equivalents
4. **Certificate Management**: Apple Developer portal, code signing, and provisioning profiles add complexity
5. **Dependency Cache**: SPM resolve can be slow without proper caching in CI

## Scope Constraints
1. **Not suitable for**: Android development, cross-platform apps (unless paired with Android agent)
2. **Limited suitability**: Apps requiring extensive background processing, file system management
3. **Not recommended**: Apps bypassing App Store (enterprise distribution limited), system modifications
4. **Restricted**: Apps using private APIs will be rejected by App Store review
