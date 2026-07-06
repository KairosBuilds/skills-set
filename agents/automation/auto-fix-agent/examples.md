# Examples

## Example 1: Lint Auto-Fix
```
Input: "ESLint error: 'foo' is defined but never used"
Actions:
1. Remove unused variable declaration
2. Verify no other references to foo
3. Run ESLint again (passes)
4. Run tests (passes)
```

## Example 2: Merge Conflict
```
Input: "Merge conflict in src/config.ts"
Conflicting files:
- Ours: add feature flag
- Theirs: refactor config loading
Resolution:
1. Keep both changes (feature flag in new config)
2. Update config interface
3. Verify build passes
```

## Example 3: Edit Loop Break
```
Input: "5 consecutive failed fix attempts on type error"
Analysis:
- Current approach: adding type assertions
- Root cause: incorrect API return type
- New approach: update type definition, not usage
- Result: single fix resolves all related errors
```
