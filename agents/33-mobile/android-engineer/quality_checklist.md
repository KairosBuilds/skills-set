# Quality Checklist — Android Engineer

## Build & Compilation
- [ ] Project compiles without errors
- [ ] `./gradlew lint` passes with zero issues
- [ ] No deprecated API usage
- [ ] R8/ProGuard release build succeeds
- [ ] APK/AAB size is within target limits
- [ ] Version code and name updated
- [ ] Manifest permissions are minimal and justified

## Functional
- [ ] App launches and renders correctly
- [ ] Navigation works for all screens
- [ ] Back navigation behaves correctly
- [ ] Configuration change (rotation) preserves state
- [ ] Dark mode renders correctly
- [ ] Network calls succeed with loading/error states
- [ ] Offline mode degrades gracefully
- [ ] Deep linking works
- [ ] Push notifications received and actionable

## Performance
- [ ] No main thread blocking (>16ms frame drops)
- [ ] Compose recomposition optimized (minimal skips)
- [ ] Cold start under 3 seconds on reference device
- [ ] Memory stable with no leaks (LeakCanary clean)
- [ ] LazyColumn/LazyGrid scrolls at 60fps
- [ ] APK size optimized (resource shrinking, R8)
- [ ] Network calls are cached appropriately

## Compatibility
- [ ] Tested on API 26 (minimum)
- [ ] Tested on API 34 (latest)
- [ ] Works on tablet form factor
- [ ] Works on different screen densities (mdpi-xxxhdpi)
- [ ] Works with RTL layouts
- [ ] Handles multi-window/split-screen

## Accessibility
- [ ] Content descriptions on all icons and images
- [ ] Touch targets >= 48dp
- [ ] Sufficient color contrast (WCAG AA)
- [ ] Focus order logical for keyboard navigation
- [ ] TalkBack correctly reads screen content

## Code Quality
- [ ] No hardcoded strings (string resources used)
- [ ] No print/Log statements in production code
- [ ] Coroutines properly scoped and cancelled
- [ ] Hilt modules properly scoped
- [ ] ViewModel StateFlow exposed as immutable
- [ ] Repository pattern followed consistently
- [ ] Error handling covers all network/data operations
- [ ] Unit tests for ViewModels and repositories
- [ ] Compose UI tests for critical flows
