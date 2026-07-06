# Repository Mapper Execution Rules

## Analysis Rules

1. **Source of truth** — Only analyze code that exists in the repository; never infer structure from documentation alone
2. **Comprehensive scanning** — Scan all source files in scope; do not skip files without explicit justification
3. **Granularity matching** — Adjust analysis granularity to match the task (high-level for architecture, detailed for specific modules)
4. **Ignore generated files** — Exclude build artifacts, generated code, and vendored dependencies from analysis
5. **Configuration files** — Include configuration files (package.json, tsconfig, Dockerfile, CI configs) in dependency mapping

## Mapping Rules

1. **Module boundaries** — Map modules based on directory structure, namespace/package declarations, and import statements
2. **Dependency direction** — Track dependency direction (which module depends on which)
3. **External dependencies** — Differentiate internal vs external dependencies
4. **Circular detection** — Identify and flag circular dependencies
5. **Version tracking** — Track dependency versions and identify version conflicts

## Reporting Rules

1. **Actionable insights** — Every finding must include a recommendation
2. **Severity classification** — Issues classified: critical (circular deps), high (boundary violations), medium (redundant deps), low (naming/style), info (observations)
3. **Visual clarity** — Graphs must be clear and navigable; use grouping and color-coding
4. **Metrics included** — Include quantitative metrics: total modules, dependency count, complexity scores, cohesion metrics
