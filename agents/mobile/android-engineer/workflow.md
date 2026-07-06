# Workflow — Android Engineer

## Phase 1: Project Initiation
1. Create Android project with Android Studio template or `gradle init`
2. Configure Kotlin and Compose compiler versions
3. Set up version catalog (libs.versions.toml)
4. Configure ProGuard/R8 rules
5. Set up lint configuration

## Phase 2: Architecture Foundation
1. Set up Hilt dependency injection modules
2. Create base classes (BaseViewModel, BaseScreen, etc.)
3. Configure Retrofit + OkHttp networking layer
4. Set up Room database with migrations
5. Implement repository pattern for data layer
6. Set up navigation graph with Compose Navigation

## Phase 3: Feature Implementation
1. Define data models and DTOs
2. Implement API services and database DAOs
3. Build repository implementations
4. Create ViewModels with StateFlow
5. Build Composable screens
6. Implement navigation between screens
7. Add loading, error, and empty state handling

## Phase 4: Testing
1. Write unit tests for ViewModels
2. Write unit tests for repositories (mocked)
3. Write Compose UI tests for critical flows
4. Write integration tests for data layer
5. Run tests on emulator API 26 and API 34

## Phase 5: Optimization
1. Profile with Android Studio Profiler
2. Optimize Compose recomposition
3. Implement Paging 3 for large lists
4. Add WorkManager for background tasks
5. Optimize APK size with R8 and resource shrinking

## Phase 6: Release
1. Update versionCode and versionName
2. Generate signed release APK/AAB
3. Test release build on physical device
4. Upload to Google Play Console
