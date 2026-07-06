# Quality Checklist — Flutter Engineer

## Build & Compilation
- [ ] `flutter analyze` passes with zero issues
- [ ] No deprecated API usage
- [ ] `flutter test` passes for all test files
- [ ] iOS release build succeeds
- [ ] Android release build succeeds
- [ ] Web build succeeds (if targeting web)
- [ ] Desktop build succeeds (if targeting desktop)

## Functional
- [ ] App launches on all target platforms
- [ ] Navigation/routing works with deep links
- [ ] All API calls handled with loading/error states
- [ ] Form validation works correctly on submit
- [ ] Keyboard handling does not overflow layout
- [ ] Back navigation correctly pops routes
- [ ] Platform back gesture (iOS swipe) works
- [ ] Pull-to-refresh works on list screens

## Performance
- [ ] No visible jank during scroll (60fps)
- [ ] List views use itemBuilder pattern
- [ ] Images display with proper caching and placeholders
- [ ] `const` constructors used wherever possible
- [ ] No unnecessary rebuilds (verified with DevTools)
- [ ] Release build does not have debug checks
- [ ] Memory usage stable over 10 minutes of use

## UI & Design
- [ ] Material 3 / Cupertino styling consistent
- [ ] Dark mode and light mode both render correctly
- [ ] Text scales properly with system font size
- [ ] Safe areas respected on notched devices
- [ ] Landscape orientation supported or properly locked
- [ ] Responsive layout works on tablets
- [ ] Fonts load correctly (google_fonts or bundled)

## Accessibility
- [ ] Semantics labels on all interactive elements
- [ ] Sufficient color contrast
- [ ] Touch targets >= 48x48dp
- [ ] Screen reader correctly describes UI
- [ ] Focus traversal order logical

## Code Quality
- [ ] No print() statements in production code
- [ ] All controllers/streams properly disposed
- [ ] Error boundaries / catch clauses handle failures
- [ ] No magic strings or numbers — constants extracted
- [ ] Widgets are composable under 200 lines
- [ ] Unit tests for business logic
- [ ] Widget tests for critical screens
- [ ] All lint rules from analysis_options.yaml followed
