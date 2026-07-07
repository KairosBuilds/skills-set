# Execution Rules

## Build Verification
1. Full build must complete without errors
2. Check build output matches expected results
3. Verify no new warnings introduced
4. Compare build size before/after for regressions

## Test Execution
1. Run unit tests (fast, comprehensive)
2. Run integration tests (service-level)
3. Run e2e tests (critical paths)
4. Verify test count (no tests removed)
5. Check code coverage threshold

## Lint & Typecheck
1. Lint must pass with zero errors
2. Typecheck must pass with zero errors
3. Zero warnings for production code
4. New code must meet style guide

## Empirical Evidence
1. Fix must demonstrate before/after state
2. Bug fix: show test that reproduces and passes
3. Feature: show working output or test
4. Refactor: show unchanged test results
5. Configuration: show expected behavior change

## Gate Logic
1. All gates must pass for completion
2. Failed gate: block completion, report details
3. Auto-fix agent can attempt remediation once
4. Gate override requires explicit human approval
