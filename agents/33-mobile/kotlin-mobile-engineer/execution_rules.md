# Execution Rules — Kotlin Mobile Engineer

## Architecture Rules
- Use Clean Architecture layers: data → domain → presentation
- Shared business logic in commonMain; platform-specific in androidMain/iosMain
- Use expect/actual declarations for platform-specific implementations
- Prefer use cases for complex business operations
- Use Repository pattern for data access in shared module

## KMP Rules
- Keep platform-specific code minimal — maximize common code
- Use `@OptionalExpectation` for Android-only interfaces
- Access iOS APIs via Kotlin/Native interop (cinterop)
- Use SKIE for better Swift interop from KMP shared code
- Test shared code on both platforms before release

## Coroutine Rules
- Use `viewModelScope` in Android; custom scopes in shared code
- Inject `CoroutineDispatcher` via expect/actual
- Prefer `Flow` over `StateFlow` in shared data layer
- Use `kotlinx-coroutines` in commonMain with `kotlinx-coroutines-android` for Android

## Networking Rules
- Use Ktor client in shared module for cross-platform networking
- Define API models in commonMain using kotlinx.serialization
- Implement token refresh as Ktor plugin
- Use expect/actual for platform-specific SSL settings

## UI Rules
- Use Compose Multiplatform for shared UI where appropriate
- Use platform-specific UI (Jetpack Compose for Android, SwiftUI for iOS) for complex scenarios
- Handle safe areas and keyboard insets per platform

## Testing Rules
- Write unit tests in commonTest for shared business logic
- Use `kotlin.test` with `kotlinx-coroutines-test`
- Test ViewModels with Turbine for Flow assertions
- Use MockK for mocking in shared tests
