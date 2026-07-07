# Workflow — iOS Engineer

## Phase 1: Project Setup
1. Choose project generation (Xcode project or XcodeGen spec)
2. Set up SPM packages
3. Configure build settings and deployment target
4. Set up linting (SwiftLint)
5. Create folder structure (feature-based or layer-based)

## Phase 2: Foundation
1. Configure app delegate / scene delegate
2. Set up dependency injection (factory or container)
3. Create networking layer (URLSession async/await)
4. Set up data persistence (SwiftData/CoreData)
5. Implement navigation/coordinator pattern
6. Configure deep linking support

## Phase 3: Feature Implementation
1. Create data models
2. Implement API service and repository
3. Build ViewModel/ObservableObject
4. Implement SwiftUI views with proper state management
5. Add animations and transitions
6. Implement error handling and empty states
7. Add haptic feedback for interactions

## Phase 4: Apple Ecosystem Integration
1. Add push notifications via APNs
2. Implement Handoff for continuity
3. Add Widget extension
4. Configure Watch companion app (if applicable)
5. Implement Share extension (if applicable)

## Phase 5: Testing
1. Write unit tests with XCTest
2. Write UI tests with XCUITest
3. Test on multiple device sizes (iPhone SE, Pro Max)
4. Test on physical device
5. Profile with Instruments

## Phase 6: Release
1. Configure app icons and assets
2. Set up App Store Connect metadata
3. Archive and upload to App Store Connect
4. Submit for TestFlight review
5. Handle App Store review feedback
