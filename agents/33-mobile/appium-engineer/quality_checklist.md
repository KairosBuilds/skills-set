# Quality Checklist — Appium Engineer

## Environment
- [ ] Appium 2.x server installed and configured
- [ ] UiAutomator2 driver installed for Android
- [ ] XCUITest driver installed for iOS
- [ ] Appium Inspector connected successfully
- [ ] Android emulator/device detected via adb
- [ ] iOS simulator/device detected via xcrun
- [ ] WDA compiled and running on iOS target
- [ ] Capabilities file externalized (not hardcoded)

## Test Structure
- [ ] Page Object Model pattern followed
- [ ] Base page class with shared methods
- [ ] Locators stored as class-level constants
- [ ] Explicit waits for all element interactions
- [ ] No Thread.sleep() in test code
- [ ] Test data separated from test logic
- [ ] Fixtures properly scoped (session/function/class)

## Test Quality
- [ ] Tests run independently (no shared state)
- [ ] Tests clean up after themselves
- [ ] Soft assertions used for non-critical checks
- [ ] Screenshots captured on failure
- [ ] Page transitions awaited with proper conditions
- [ ] Scrolling logic handles various screen sizes
- [ ] Keyboard handling works correctly

## Cross-Platform
- [ ] Tests run on Android emulator
- [ ] Tests run on iOS simulator
- [ ] Platform-specific locators isolated
- [ ] Gesture automation works on both platforms
- [ ] Alert handling for both Android and iOS
- [ ] Permission dialogs handled per platform

## Reporting & CI
- [ ] Allure report generated after test run
- [ ] Test results include environment info
- [ ] CI pipeline runs mobile tests
- [ ] Parallel execution configured (if applicable)
- [ ] Flaky test detection and retry configured
- [ ] Test results published to dashboard

## Code Quality
- [ ] No hardcoded device capabilities
- [ ] No hardcoded timeouts
- [ ] Logging captures relevant test steps
- [ ] Page objects have clear method names
- [ ] No duplication of locators across page objects
- [ ] Tests cover happy path and error cases
- [ ] Test coverage report generated
- [ ] Lint passes (pylint/flake8 for Python)
