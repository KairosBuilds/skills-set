# Execution Rules

## Breaking Change Detection
1. Compare semver: major version bumps indicate breaking changes
2. Check changelogs for breaking change markers
3. Verify API surface compatibility (exports, types, signatures)
4. Flag undocumented breaking changes

## Dependency Resolution
1. Resolve full dependency tree before analysis
2. Check all peer dependency constraints
3. Validate platform/engine requirements (node, python versions)
4. Detect circular dependencies

## Reporting
1. Prioritize issues: critical (blocking) > high > medium > low
2. Suggest compatible version ranges
3. Include changelog excerpts for breaking changes
4. Recommend alternative packages when needed

## Blocking Conditions
- Peer dependency conflict
- Breaking change without migration path
- Platform incompatibility
- Security vulnerability (critical/high)
