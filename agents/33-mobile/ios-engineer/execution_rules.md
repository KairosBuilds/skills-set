# Execution Rules — iOS Engineer

## Build Rules
- Use Swift Package Manager (SPM) as the primary dependency manager; fall back to CocoaPods only when SPM unavailable
- Set Swift Language Version to 5.9+ in build settings
- Enable `SWIFT_STRICT_CONCURRENCY` for Sendable checking
- Use XcodeGen for project files in CI environments
- Always test on physical device before marking work complete

## Architecture Rules
- Prefer SwiftUI for new UI; UIKit for complex custom interactions
- Follow MVVM or TCA (The Composable Architecture) patterns
- Use Coordinator pattern for UIKit navigation
- Keep ViewModels as observable objects with `@Published` properties
- Separate business logic into services/repositories

## Concurrency Rules
- Use Swift async/await for all async operations
- Mark classes with `@MainActor` when updating UI
- Use `actor` for shared mutable state
- Prefer `AsyncSequence` over Combine for streams
- Never use `DispatchQueue.main.async` in new code — use `MainActor`

## Data Persistence Rules
- Use SwiftData for new apps (iOS 17+); Core Data for iOS 16 and below
- Prefer `Codable` + file storage for simple data
- Use CloudKit for cross-device sync
- Cache network responses with URLCache

## Security Rules
- Use Keychain Services for sensitive tokens
- Never log user data or credentials (use OSLog with privacy)
- Implement App Attest for high-security features
- Use Data Protection API for file-level encryption

## App Store Compliance
- Support Dynamic Type for accessibility
- Implement VoiceOver support for all views
- Handle all iPad multitasking modes
- Support Dark Mode and Light Mode
