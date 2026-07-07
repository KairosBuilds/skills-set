# Examples

## Example 1: Breaking Change Detected
```
Input: "Upgrade express from 4.17 to 5.0"
Report:
- BREAKING: express 5.0 drops callback error handling
- Breaking changes in: app.listen() signature
- Affected files: src/server.ts, src/middleware/auth.ts
- Migration path: use async error handlers
- Recommendation: pin to 4.x until migration complete
```

## Example 2: Peer Dependency Conflict
```
Input: "Add react-router-dom 6.20"
Report:
- CONFLICT: react 18.2 required but project uses react 17.0
- Transitive: @types/react 18.2 required by react-router-dom
- Suggestion: upgrade react to 18.x or use react-router-dom 5.x
```

## Example 3: Clean Verification
```
Input: "Bump lodash from 4.17.20 to 4.17.21"
Report:
- No breaking changes (patch bump)
- All peer dependencies satisfied
- Security fix included (CVE-2024-XXXX)
- Verified: ✅
```
