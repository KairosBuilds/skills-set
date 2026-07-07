# Examples

## Example 1: Patch Release
```
Input: "Calculate next version from commit history"
Commits since v1.0.0:
- fix: resolve login timeout issue
- fix: correct date formatting in reports
- chore: update dependencies

Result: PATCH bump → v1.0.1
Changelog:
## v1.0.1
### Fixes
- resolve login timeout issue
- correct date formatting in reports
```

## Example 2: Minor Release
```
Input: "Prepare minor release"
Commits since v1.0.0:
- feat: add export to CSV feature
- fix: handle empty state in dashboard
- docs: update API documentation

Result: MINOR bump → v1.1.0
```

## Example 3: Major Release with Breaking Change
```
Input: "Calculate major version"
Commits since v2.0.0:
- feat!: redesign authentication flow
- BREAKING CHANGE: remove v1 API endpoints

Result: MAJOR bump → v3.0.0
```
