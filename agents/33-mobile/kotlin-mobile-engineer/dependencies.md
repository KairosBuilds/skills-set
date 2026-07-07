# Dependencies — Kotlin Mobile Engineer

## Core
- kotlin-multiplatform (Kotlin 1.9.x / 2.0.x)
- kotlinx-coroutines-core
- kotlinx-serialization-json
- kotlinx-datetime

## Shared Networking
- ktor-client-core
- ktor-client-content-negotiation
- ktor-client-serialization
- ktor-client-logging
- ktor-client-auth

## Platform Networking
- ktor-client-okhttp (Android)
- ktor-client-darwin (iOS)

## Data Storage
- sqldelight (cross-platform SQLite)
- kotlinx-datetime
- multiplatform-settings (SharedPreferences / NSUserDefaults)

## UI (Shared)
- compose-multiplatform (Compose for iOS + Android)
- compose-foundation
- compose-material3

## Dependency Injection
- koin (multiplatform DI)
- kotlin-inject (experimental)

## Architecture
- moko-mvvm (shared ViewModels)
- decompose (component-based architecture)
- voyager (multiplatform navigation)

## Testing
- kotlin-test
- kotlinx-coroutines-test
- mockk (multiplatform)
- turbine (Flow testing)
- compose-ui-test

## Build
- android-gradle-plugin
- cocoapods-gradle-plugin
- skie (Swift/Kotlin interop)
