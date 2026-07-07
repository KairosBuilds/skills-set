# Quality Checklist — Kotlin Mobile Engineer

## Build & Compilation
- [ ] Shared module compiles for Android target
- [ ] Shared module compiles for iOS target
- [ ] Android app assembles successfully
- [ ] iOS framework exports and compiles in Xcode
- [ ] Gradle build without deprecation warnings
- [ ] No unused expect/actual declarations
- [ ] kotlinx.serialization compiles correctly

## Functional
- [ ] Shared logic behaves identically on both platforms
- [ ] Network calls succeed on both platforms
- [ ] Data persistence works cross-platform
- [ ] Platform-specific UI renders native feel
- [ ] Navigation parity between Android and iOS
- [ ] Deep linking works on both platforms

## Performance
- [ ] Cold start within acceptable range on both platforms
- [ ] No excessive GC pauses on Android
- [ ] Ktor client connection pooling optimized
- [ ] SQLDelight queries are efficient
- [ ] Serialization/deserialization is performant
- [ ] Coroutine scope properly managed per platform

## Code Organization
- [ ] commonMain contains all shared business logic
- [ ] platform-specific expect/actual minimal and well-documented
- [ ] Clean Architecture layers respected
- [ ] Dependency injection configured per platform
- [ ] Only essential dependencies in commonMain

## Code Quality
- [ ] No hardcoded strings — use resource files per platform
- [ ] Consistent error handling across platforms
- [ ] All public APIs documented with KDoc
- [ ] No Kotlin deprecation warnings
- [ ] Common test coverage >= 75%
- [ ] Platform test coverage for integration points
- [ ] Lint passes on both Android and iOS modules
- [ ] Strict Kotlin compiler warnings enabled

## Platform Parity
- [ ] Feature set identical on Android and iOS
- [ ] UI behavior matches platform conventions
- [ ] Error messages consistent across platforms
- [ ] Loading/empty/error states handled equally
- [ ] Accessibility support on both platforms
