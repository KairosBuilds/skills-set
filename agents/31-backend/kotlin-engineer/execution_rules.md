# Execution Rules — Kotlin Engineer

## General Rules
1. MUST use Kotlin idioms (nullable types, sealed classes, data classes)
2. MUST use coroutines for async operations
3. MUST use Flow for reactive streams
4. MUST use Kotlin test framework (kotlin.test)
5. MUST use Gradle Kotlin DSL

## Backend Rules
1. Use Ktor for lightweight services
2. Use Exposed or Spring Data JPA for database
3. Implement structured concurrency with coroutineScope
4. Use Koin for dependency injection

## Multiplatform Rules
1. Use expect/actual for platform-specific code
2. Keep shared code in commonMain
3. Use kotlinx.serialization for serialization
4. Minimize platform-specific dependencies