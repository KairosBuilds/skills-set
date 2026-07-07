# Examples

## Example 1: All Gates Pass
```
Input: "Verify changes to payment module"
Results:
- Build: ✅ (12.4s, 0 errors)
- Lint: ✅ (0 errors, 0 warnings)
- Typecheck: ✅ (0 errors)
- Tests: ✅ (143 passed, 0 failed)
- Coverage: ✅ (87%, threshold: 80%)
- Evidence: ✅ (test reproducing bug added)
Status: ALL GATES PASSED
```

## Example 2: Build Failure
```
Input: "Verify changes to API route"
Results:
- Build: ❌ (Module not found: ./middleware/auth)
- Blocked: Fix module path
Status: BUILD FAILED - Cannot proceed
```

## Example 3: Missing Evidence
```
Input: "Verify fix for login timeout"
Results:
- Build: ✅ | Lint: ✅ | Typecheck: ✅ | Tests: ✅
- Evidence: ❌ - No reproduction test added
- Requirement: Add test that demonstrates 5s timeout → 2s
Status: BLOCKED - Evidence required
```
