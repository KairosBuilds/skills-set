# Limitations — Appium Engineer

## Technical Limitations
1. **Speed**: Appium tests run slower than Espresso/XCUITest as they use black-box automation
2. **Flakiness**: Element locators break with UI changes; XPath-based tests are especially brittle
3. **iOS Real Device**: XCUITest on physical iOS devices requires additional setup (trust, provisioning)
4. **Gesture Reliability**: Complex gestures (pinch, rotate) have varying reliability across devices
5. **App State**: Cannot test background system features (push notifications arrive while app backgrounded)
6. **Biometrics**: Face ID / Touch ID testing requires simulator-specific configuration
7. **Performance Testing**: Appium is not suitable for performance benchmarking (adds overhead)

## Process Limitations
1. **Setup Complexity**: Requires Appium server, driver-specific dependencies, and platform toolchains
2. **Slow Feedback**: Mobile E2E tests take 2-10x longer than their web equivalents
3. **Device Fragmentation**: Need access to multiple real devices for comprehensive coverage
4. **iOS Build Requirement**: WDA must be compiled against the same Xcode version
5. **Maintenance Burden**: UI changes in the app often require test updates

## Scope Constraints
1. **Not suitable for**: Unit testing, integration testing (use platform-native frameworks)
2. **Limited suitability**: Performance benchmarking, load testing, API-only testing
3. **Not recommended**: Testing apps without UI, testing system-level features, accessibility audits
4. **Cannot test**: Push notification delivery (can test response), system dialogs (limited), cross-app interactions
5. **Weekend/Flaky**: Tests may fail due to network conditions, device state, or timing issues
