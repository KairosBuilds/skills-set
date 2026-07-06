# Workflow — Appium Engineer

## Phase 1: Environment Setup
1. Install Appium 2.x (`npm install -g appium`)
2. Install drivers: `appium driver install uiautomator2` and `appium driver install xcuitest`
3. Install Appium Inspector for element inspection
4. Set up Android emulator / iOS simulator
5. Configure cloud provider (if applicable: BrowserStack, Saucelabs)

## Phase 2: Project Setup
1. Initialize Python project with pytest
2. Create conftest.py with driver fixtures
3. Set up Page Object Model directory structure
4. Install dependencies (Appium-Python-Client, pytest, allure-pytest)
5. Create base page class with common methods

## Phase 3: Page Object Implementation
1. Inspect app elements with Appium Inspector
2. Create page classes for each screen
3. Implement locators as class-level tuples
4. Add action methods with explicit waits
5. Create assertion methods

## Phase 4: Test Case Implementation
1. Write test cases with pytest
2. Use parameterization for data-driven tests
3. Implement setup/teardown fixtures
4. Add Allure annotations for reporting
5. Handle platform-specific test variations

## Phase 5: Execution
1. Run tests locally on emulator/simulator
2. Run on physical devices
3. Execute parallel test sessions
4. Record test execution video
5. Generate Allure report

## Phase 6: CI Integration
1. Configure GitHub Actions/GitLab CI for mobile tests
2. Set up Appium service in CI containers
3. Connect to cloud provider for device matrix
4. Configure test reporting dashboard
5. Set up flaky test detection and retry

## Phase 7: Maintenance
1. Review test stability metrics weekly
2. Update locators on app UI changes
3. Refactor flaky tests
4. Update Appium and driver versions
5. Expand test coverage for new features
