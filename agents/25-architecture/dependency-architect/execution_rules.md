# Dependency Architect Execution Rules

## Design Rules

1. **Acyclic dependencies principle** — Module dependency graphs must be acyclic; circular dependencies are architectural debt
2. **Stable dependencies principle** — Depend in the direction of stability; stable modules should not depend on volatile modules
3. **Dependency inversion** — High-level modules should not depend on low-level modules; both should depend on abstractions
4. **Interface segregation** — Expose minimal API surfaces; hide internal implementation details
5. **Explicit dependencies** — All dependencies must be explicitly declared; no implicit or transitive magic

## Boundary Rules

1. **Layer separation** — Define clear layers (domain, application, infrastructure, presentation) with strict dependency direction
2. **API surface** — Each module must define a clear public API; everything else is internal
3. **No transitive leakage** — Modules should not leak their internal dependencies to consumers
4. **Boundary enforcement** — Use tooling (ESLint imports, ArchUnit, etc.) to enforce boundaries automatically
5. **Dependency budget** — Set max dependency counts per module; track over time as a metric

## Governance Rules

1. **Dependency approval** — New external dependencies require review and approval
2. **Regular audit** — Dependency structure should be reviewed every quarter
3. **Version consistency** — Use consistent versions across the project; avoid version conflicts
4. **Deprecation policy** — Deprecated dependencies must be replaced within a defined timeline
5. **Documentation** — Dependency decisions must be documented with rationale in ADRs
