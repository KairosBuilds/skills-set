# Repository Mapper Examples

## Example 1: Full Codebase Map

**Request:** "Map our entire frontend monorepo"

**Output:**
- Structure: 5 packages (core, ui, api-client, admin, app) with 247 TypeScript files
- Dependencies: 120 internal dependencies, 340 external dependencies
- Circular deps: 3 found — all in ui package (2 resolved with refactoring suggestions)
- Metrics: Average fan-in 3.2, average fan-out 4.1, highest coupled module: shared/utils
- Visualization: Mermaid dependency graph with color-coded packages
- Recommendation: Split shared/utils to reduce coupling, extract 2 cycles into new package

## Example 2: Module Boundary Audit

**Request:** "Check if our clean architecture boundaries are being violated"

**Analysis:**
- Intended: Domain → Application → Infrastructure → Presentation
- Found: 12 violations where Infrastructure imports Application directly
- Found: 4 cases where domain layer has external framework dependencies
- Report: Violations by severity — 2 critical, 5 high, 3 medium, 2 low
- Recommendation: Add architecture tests to enforce boundary rules, fix critical violations first

## Example 3: Dependency Analysis for Refactoring

**Request:** "Which modules will break if we replace our HTTP library?"

**Analysis:**
- Impact: 47 files across 3 packages directly import the HTTP library
- Secondary: 89 additional files depend on classes that use the HTTP library
- Map: Detailed change impact diagram showing affected modules
- Suggestion: Introduce an HTTP abstraction layer to minimize future migration pain
