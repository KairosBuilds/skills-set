# Execution Rules — Flutter Engineer

## Build Rules
- Run `flutter clean` and `flutter pub get` when switching feature branches
- Use `flutter analyze` before every commit — treat all warnings as errors
- Enable `const` constructors wherever possible to improve performance
- Prefer `--split-debug-info` and `--obfuscate` for release builds
- Use code generation (build_runner) for JSON serialization, routing, and state code

## Code Quality Rules
- All widget trees must be cleanly composable — avoid widgets over 200 lines
- Use `const` constructors for all widgets that don't mutate
- Prefer composition over inheritance — use mixins and extensions
- Extract reusable widgets into separate files early
- Use `value_notifier` or `change_notifier` for local state; Riverpod for global
- Always dispose controllers and subscriptions in `dispose()`

## Performance Rules
- Use `RepaintBoundary` around animated widgets
- Avoid `Opacity` widget for entire subtrees; prefer `AnimatedOpacity`
- Use `const` widgets to enable Flutter's canonicalize
- Prefer `ListView.builder` over `ListView` for dynamic lists
- Use `ItemExtent` in ListView for fixed-size items
- Profile with Flutter DevTools before marking performance work done

## State Management Rules
- Prefer Riverpod 2.x over BLoC for new projects
- Use `flutter_bloc` for complex event-driven flows
- Never put business logic in widgets — use Controllers/Notifiers
- Keep providers scoped — avoid global providers for local UI state

## Platform Rules
- Use `dart:io` platform checks sparingly; prefer `Platform` from `foundation`
- Conditionally import platform-specific implementations with `default_target_platform`
- Use `MethodChannel` for communication with native platform code
- Handle keyboard insets and safe areas with `MediaQuery` and `SystemChrome`
