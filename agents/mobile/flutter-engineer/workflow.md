# Workflow — Flutter Engineer

## Phase 1: Setup & Planning
1. Create Flutter project (`flutter create --org com.company.appname`)
2. Configure analysis_options.yaml with strict lint rules
3. Set up folder structure (feature-first or layer-first)
4. Choose state management (Riverpod or BLoC)
5. Plan widget composition and component hierarchy

## Phase 2: Foundation
1. Set up theming (ThemeData, ColorScheme, TextTheme)
2. Configure routing (go_router or auto_route)
3. Set up dependency injection
4. Implement API client with Dio
5. Configure localization (flutter_localizations + intl)

## Phase 3: Feature Implementation
1. Create data models with freezed + json_serializable
2. Implement repository pattern
3. Build state providers/notifiers
4. Create widget components following composition pattern
5. Add animations (Hero, AnimatedContainer, staggered)
6. Implement form validation

## Phase 4: Platform Integration
1. Add platform-specific plugins (camera, location, etc.)
2. Implement platform channels for custom native functionality
3. Configure deep linking
4. Set up push notifications
5. Handle background tasks

## Phase 5: Testing
1. Write unit tests for models and controllers
2. Write widget tests for critical components
3. Write integration tests for full flows
4. Test on multiple screen sizes and platforms
5. Run on physical devices

## Phase 6: Release
1. Configure app icons and splash screen
2. Set up code signing
3. Build release artifacts for target platforms
4. Run integration tests on release build
5. Deploy to stores
