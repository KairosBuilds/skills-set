# Workflow — React Native Engineer

## Phase 1: Requirements Analysis
1. Identify target platforms (iOS, Android, or both)
2. Determine required native modules vs pure JS solutions
3. Choose navigation library (React Navigation or Expo Router)
4. Decide state management approach
5. Plan offline/offline-first strategy

## Phase 2: Project Setup
1. Initialize project (`npx create-expo-app` or `npx react-native init`)
2. Configure TypeScript strict mode
3. Set up Metro bundler with custom config
4. Install essential dependencies (navigation, state, networking)
5. Configure ESLint + Prettier
6. Set up Jest + React Native Testing Library

## Phase 3: Implementation
1. Build component tree following atomic design
2. Implement navigation structure (stacks, tabs, drawers)
3. Create API layer with React Query
4. Implement state management stores
5. Build UI components with proper keyboard handling
6. Add animations with Reanimated + Gesture Handler

## Phase 4: Native Module Integration
1. Write TypeScript interface for native module
2. Implement iOS native code (Swift/Obj-C)
3. Implement Android native code (Kotlin/Java)
4. Generate types with Codegen
5. Test on both platforms

## Phase 5: Testing
1. Write unit tests for utilities and stores
2. Write component tests with React Native Testing Library
3. Write integration tests for critical flows
4. Write E2E tests with Detox for critical paths
5. Test on physical devices (minimum: iPhone SE, Pixel 6)

## Phase 6: Build & Release
1. Configure app icons and splash screen
2. Set up code signing (Apple Developer + Google Play)
3. Build for staging with staging env
4. Run E2E tests on release build
5. Submit to TestFlight + Internal Track

## Phase 7: Monitoring
1. Set up Crashlytics or Sentry
2. Configure performance monitoring
3. Set up remote error logging
4. Review analytics for regression
