# Execution Rules — React Native Engineer

## Build Rules
- Always clear Metro cache (`npx react-native start --reset-cache`) when switching branches or after native dependency changes
- Run `npx pod-install` after adding native modules (iOS)
- Use Hermes engine for production builds; enable via `hermes: true` in `metro.config.js`
- Prefer new architecture (Fabric + TurboModules) for new projects
- Use Codegen for typed native modules

## Code Quality Rules
- All components must have TypeScript strict mode enabled
- Avoid inline styles in production code; use StyleSheet.create or styled-components
- Memoize expensive computations with useMemo and useCallback
- FlatList over ScrollView for lists of unknown length
- Use React.memo for pure components that re-render often
- Prefer functional components with hooks over class components
- Handle loading, error, and empty states for every async operation

## Performance Rules
- Profile with Hermes CLI and Flipper before marking work done
- Lazy load screens with React.lazy or @react-navigation lazy
- Optimize images with expo-image or react-native-fast-image
- Reduce bridge traffic by batching native calls
- Use InteractionManager.runAfterInteractions for heavy post-navigation work

## State Management Rules
- Prefer Zustand or Jotai over Redux for new projects
- Use React Query (TanStack Query) for server-state
- Persist only essential state with AsyncStorage
- Avoid prop-drilling deeper than 3 levels

## Security Rules
- Never store secrets in JS bundle; use environment variables via react-native-config
- Sanitize WebView input with allowed origin/domain whitelists
- Use react-native-encryption for sensitive local data
- Pin SSL certificates for production API calls
