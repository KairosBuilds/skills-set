# Quality Checklist — iOS Engineer

## Build & Compilation
- [ ] Xcode build succeeds without errors
- [ ] SwiftLint passes with zero violations
- [ ] No deprecated API usage
- [ ] Archive succeeds for App Store distribution
- [ ] Code signing and provisioning profiles valid
- [ ] App icon and assets configured correctly
- [ ] Info.plist entries complete and accurate

## Functional
- [ ] App launches and renders correctly
- [ ] Navigation works with proper back swipe gesture
- [ ] Deep links route to correct screens
- [ ] Push notifications received and actionable
- [ ] State restoration works after app termination
- [ ] Handoff continuity works (if applicable)
- [ ] Dynamic Type text sizing works correctly
- [ ] Dark mode and light mode both render correctly

## Performance
- [ ] Cold start under 2 seconds on reference device (iPhone 14)
- [ ] Scroll performance at 60fps (120fps for ProMotion)
- [ ] Memory usage stable — no leaks (Instruments clean)
- [ ] Energy impact — no excessive background activity
- [ ] Network requests use caching appropriately
- [ ] Image loading is lazy with proper placeholders
- [ ] Animation frame rate consistent

## Compatibility
- [ ] Tested on iPhone SE (small screen)
- [ ] Tested on iPhone Pro Max (large screen)
- [ ] Tested on iPad (multitasking)
- [ ] Tested on physical device
- [ ] Landscape orientation supported or properly locked
- [ ] iOS 16 and iOS 17 both supported
- [ ] RTL language support (if localized)

## Accessibility
- [ ] VoiceOver describes all elements correctly
- [ ] Dynamic Type scales all text
- [ ] Sufficient color contrast (WCAG AA)
- [ ] Reduced Motion respected
- [ ] Focus indicators visible for keyboard navigation
- [ ] Touch targets >= 44x44pt

## Code Quality
- [ ] No force unwraps (!) in production code
- [ ] No print/NSLog statements
- [ ] All async calls use proper error handling
- [ ] @MainActor used on all UI-updating code
- [ ] Actors protect shared mutable state
- [ ] Unit tests pass for all model/business logic
- [ ] UI tests cover critical user flows
- [ ] Test coverage >= 80%
- [ ] Sendable annotations where needed
