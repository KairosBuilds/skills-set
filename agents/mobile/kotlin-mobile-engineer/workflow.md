# Workflow — Kotlin Mobile Engineer

## Phase 1: Project Setup
1. Create KMP project with KMP wizard or template
2. Configure Gradle with Kotlin Multiplatform plugin
3. Set up shared, androidApp, iosApp modules
4. Configure version catalog for dependencies
5. Set up kotlinx.serialization

## Phase 2: Shared Module
1. Define domain models in commonMain
2. Implement repository interfaces
3. Create Ktor API client in commonMain
4. Write expect declarations for platform APIs
5. Implement actual declarations in androidMain and iosMain
6. Write shared use cases and business logic

## Phase 3: Android App
1. Set up Jetpack Compose with Material 3
2. Implement Hilt dependency injection
3. Create Compose screens consuming shared ViewModels
4. Implement Android-specific features (notifications, widgets)
5. Build navigation with Compose Navigation

## Phase 4: iOS App
1. Configure KMP framework export for iOS
2. Build SwiftUI wrapper around shared KMP code
3. Implement iOS-specific UI with native components
4. Integrate with iOS system features

## Phase 5: Compose Multiplatform (Optional)
1. Set up Compose Multiplatform targets
2. Share UI components for simple screens
3. Use platform-specific CompositionLocals where needed
4. Build navigation compatible with both platforms

## Phase 6: Testing
1. Write common tests in commonTest for shared logic
2. Run Android instrumentation tests
3. Test iOS integration via XCUITest
4. Verify behavior parity across platforms

## Phase 7: Distribution
1. Build Android release AAB
2. Build iOS framework and generate XCFramework
3. Configure CI for both platforms
4. Publish Android to Play Store and iOS to App Store
