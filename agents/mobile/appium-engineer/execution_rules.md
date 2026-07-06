# Execution Rules — Appium Engineer

## Setup Rules
- Install Appium 2.x globally and per-project dependently via @appium/base-driver
- Use appium-installer or appium-setup for quick environment configuration
- Use UiAutomator2 as the default Android driver
- Use XCUITest as the default iOS driver
- Configure capabilities from environment variables, never hardcoded

## Locator Strategy Rules
- Prefer accessibility IDs over XPath for performance and stability
- Use `-ios predicate string` and `-android uiautomator` for complex queries
- Avoid absolute XPath — use relative/partial locators
- Use data-testid attributes where available in the app
- Implement explicit waits for all element interactions (WebDriverWait)

## Test Design Rules
- Follow Page Object Model (POM) for all test projects
- One assertion per test method (single responsibility)
- Use pytest fixtures for driver setup and teardown
- Keep tests independent — never depend on test order
- Use soft assertions for non-blocking validation when appropriate

## Driver Management Rules
- Initialize Appium driver in a session-level fixture
- Quit driver in teardown to release resources
- Use RemoteWebDriver for cloud providers (Saas Labs, BrowserStack)
- Handle app state: terminate, activate, background appropriately
- Set implicit wait globally; override with explicit waits for individual elements

## Platform-Specific Rules
- iOS: Use Xcode build for WDA (WebDriverAgent) compilation
- Android: Ensure ADB server is running and device/emulator is authorized
- iOS Simulator: Use `platformVersion` matching Xcode SDK
- Android Emulator: Use `avd` capability for automatic AVD launch

## Reporting Rules
- Integrate Allure for test reporting
- Capture screenshots on test failure automatically
- Log Appium server logs on failure for debugging
- Record video for flaky test analysis
