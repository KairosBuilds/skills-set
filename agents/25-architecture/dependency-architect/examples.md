# Dependency Architect Examples

## Example 1: Circular Dependency Resolution

**Request:** "We have a circular dependency between our auth and user modules"

**Analysis:**
- Cycle: auth → user → shared → auth
- Root cause: auth module imports from shared, which imports from auth for type definitions
- Resolution: Extract common types into a new `@core/types` package, removing the cycle
- Impact: 5 files changed, no behavioral change, zero-downtime migration possible
- Prevention: Add ESLint rule `import/no-cycle` to prevent future cycles

## Example 2: Dependency Governance Policy

**Request:** "Create a dependency management policy for our project"

**Output:**
```
## Dependency Rules
1. All new external dependencies require an ADR
2. No circular dependencies allowed (CI blocks)
3. Module layers: domain → application → infrastructure → presentation (enforced via ArchUnit)
4. Each module max 10 direct internal dependencies, 20 external
5. Version pinning: use exact versions for production dependencies
6. Quarterly dependency audit required
7. Deprecated dependencies must be replaced within 6 months
```

## Example 3: Module Boundary Violation Audit

**Request:** "Check for leaning module boundaries in our monorepo"

**Findings:**
- 23 boundary violations found (8 critical, 10 high, 5 medium)
- Most common: infrastructure modules importing presentation types
- Critical: Shared UI library importing from admin-specific module
- Automated fix: Add import restrictions in ESLint config
- Manual fix: Extract shared types, refactor 3 modules
- Timeline: 1 sprint for critical fixes, 2 sprints for all violations
