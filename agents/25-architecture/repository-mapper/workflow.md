# Repository Mapper Workflow

## Standard Mapping Flow

### Phase 1: Repository Scan
1. Discover repository structure
2. Identify all source files and their types
3. Read configuration files (package.json, tsconfig, etc.)
4. Map directory structure

### Phase 2: Dependency Extraction
1. Scan import/require/include statements across all files
2. Extract internal module dependencies
3. Extract external dependency references
4. Build comprehensive dependency list

### Phase 3: Graph Construction
1. Build dependency graph (nodes = modules, edges = dependencies)
2. Identify circular dependencies
3. Calculate dependency metrics (fan-in, fan-out, depth)
4. Highlight critical paths and bottlenecks

### Phase 4: Boundary Analysis
1. Compare actual architecture against intended boundaries
2. Identify boundary violations
3. Detect layering violations
4. Assess module cohesion and coupling

### Phase 5: Reporting
1. Generate directory tree with annotations
2. Create dependency graph visualization
3. List findings with severity ratings
4. Provide actionable recommendations

## Output Template

```
1. Repository Overview
2. Directory Structure
3. Module Catalog
4. Dependency Graph
5. Circular Dependencies (if found)
6. Module Boundary Analysis
7. Dead Code Analysis
8. Change Impact Map
9. Metrics Summary
10. Recommendations
```
