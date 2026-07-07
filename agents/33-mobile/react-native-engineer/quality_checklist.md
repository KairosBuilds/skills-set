# Quality Checklist — React Native Engineer

## Build & Compilation
- [ ] Metro bundler succeeds without warnings
- [ ] TypeScript strict mode passes with zero errors
- [ ] iOS build succeeds (xcodebuild / expo run:ios)
- [ ] Android build succeeds (gradle / expo run:android)
- [ ] Hermes bytecode compilation succeeds
- [ ] Production bundle size < 25MB (release APK/IPA)

## Functional
- [ ] App launches and renders initial screen
- [ ] Navigation works across all routes and deep links
- [ ] All API calls succeed with loading/error/empty states
- [ ] Offline mode gracefully degrades
- [ ] Push notifications received and handled correctly
- [ ] Keyboard handling does not obscure inputs
- [ ] Back navigation behaves as expected (Android hardware back)
- [ ] All gestures (swipe, pinch, tap) work as intended

## Performance
- [ ] FlatList/VirtualizedList scroll at 60fps
- [ ] No unnecessary re-renders (verified with React DevTools profiler)
- [ ] App cold start under 3 seconds on reference device (Pixel 6)
- [ ] JS thread does not block for >100ms during transitions
- [ ] Images lazy loaded with placeholders
- [ ] Memory usage stable during extended use (no leaks)
- [ ] Animation frames consistently at 60fps

## Cross-Platform
- [ ] Tested on iOS (iPhone SE, iPhone 15)
- [ ] Tested on Android (Pixel 6, Samsung Galaxy S23)
- [ ] Safe areas handled correctly (notch, Dynamic Island)
- [ ] Platform-specific code properly conditionally applied
- [ ] Font rendering consistent across platforms
- [ ] Shadow/elevation rendering matches design

## Accessibility
- [ ] Screen reader support (accessibilityLabel, accessibilityRole)
- [ ] Touch targets minimum 44x44pt
- [ ] Sufficient color contrast ratios
- [ ] Reduced motion respected for animations
- [ ] Focus management for keyboard navigation

## Security
- [ ] API keys and secrets not in bundled code
- [ ] WebView sandboxed and origin-restricted
- [ ] Deep link URL validation
- [ ] Certificate pinning for production APIs
- [ ] Secure storage used for tokens and PII

## Code Quality
- [ ] No console.log in production code
- [ ] Error boundaries at each navigation level
- [ ] PropTypes or TypeScript types for all component props
- [ ] No hardcoded strings (i18n ready)
- [ ] Tests cover critical user flows
- [ ] Code follows team linting and formatting rules
