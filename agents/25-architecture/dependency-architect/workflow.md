# Dependency Architect Workflow

## Standard Analysis Flow

### Phase 1: Dependency Discovery
1. Scan codebase for all dependencies (internal and external)
2. Catalog dependencies by type (direct, transitive, dev, peer)
3. Build dependency matrix
4. Identify dependency versions

### Phase 2: Structure Analysis
1. Map module dependency graph
2. Measure coupling metrics (afferent, efferent, instability)
3. Identify circular dependencies and violations
4. Assess module layering compliance

### Phase 3: Boundary Analysis
1. Define or validate module API surfaces
2. Check boundary compliance
3. Identify leaky abstractions
4. Detect transitive dependency leakage

### Phase 4: Optimization Planning
1. Prioritize dependency issues by severity
2. Design refactoring strategy for circular dependencies
3. Plan boundary enforcement improvements
4. Create dependency reduction roadmap

### Phase 5: Governance Design
1. Define dependency rules and policies
2. Design automated enforcement (lint rules, CI checks)
3. Create dependency review process
4. Document governance policy

### Phase 6: Reporting
1. Compile dependency analysis report
2. Include metrics and visualizations
3. Provide prioritized recommendations
4. Create governance policy document

## Output Template

```
1. Dependency Overview
2. Dependency Matrix
3. Module Dependency Graph
4. Coupling Metrics
5. Circular Dependency Analysis
6. Boundary Violations
7. Version Conflict Analysis
8. Optimization Recommendations
9. Governance Policy
10. Implementation Roadmap
```
