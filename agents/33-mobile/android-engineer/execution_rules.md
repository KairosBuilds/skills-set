# Execution Rules — Android Engineer

## Build Rules
- Prefer Kotlin over Java for all new code
- Use Gradle Kotlin DSL (build.gradle.kts) for build configurations
- Enable R8 full mode for release builds
- Use version catalogs (libs.versions.toml) for dependency management
- Run `./gradlew lint` before committing

## Architecture Rules
- Follow MVVM or MVI architecture pattern
- Use Repository pattern for data access
- Keep Activities/Fragments thin — logic in ViewModels
- Use Unidirectional Data Flow (UDF) with StateFlow
- Prefer single-Activity architecture with Jetpack Navigation

## Dependency Injection Rules
- Use Hilt for dependency injection
- Scope dependencies appropriately (Singleton, ViewModelScoped, FragmentScoped)
- Never inject Application context where Activity context suffices

## Concurrency Rules
- Use Kotlin Coroutines + Flow for async operations
- Use Dispatchers.IO for network and disk operations
- Never call blocking code on the main thread
- Cancel coroutine scopes on lifecycle destroy

## UI Rules
- Prefer Jetpack Compose over XML layouts for new UIs
- Use Material 3 design components
- Support dark mode via dynamic color theming
- Handle configuration changes without state loss (rememberSavable, ViewModel)
- Use LazyColumn/LazyGrid for scrollable content

## Security Rules
- Use EncryptedSharedPreferences for sensitive data
- Never log PII or auth tokens
- Use ProGuard/R8 mapping files for crash reporting
- Implement certificate pinning with OkHttp
