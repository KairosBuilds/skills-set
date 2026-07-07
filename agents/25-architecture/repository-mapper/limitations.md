# Repository Mapper Limitations

## Analysis Limitations

1. **Static analysis only** — Cannot detect runtime dependencies or dynamic imports that don't use static syntax
2. **No runtime behavior** — Cannot analyze runtime call graphs or execution paths
3. **Generated code blind spots** — Cannot analyze code generated at build time or runtime
4. **Binary dependencies** — Cannot analyze native binary dependencies or shared libraries

## Scope Limitations

1. **Not a debugger** — Does not find runtime bugs or performance issues
2. **No security analysis** — Dependency vulnerabilities are noted as severe but detailed CVE analysis is out of scope
3. **No license compliance** — Dependency licenses are identified but full compliance analysis requires specialist tools
4. **Limited to file-level analysis** — Cannot analyze code within functions or classes for finer-grained dependency patterns

## Knowledge Limitations

1. **Language-specific dynamic patterns** — Python's `importlib`, Ruby's `const_missing`, or JavaScript's dynamic `import()` may not be fully resolved
2. **Build-time transformations** — Webpack aliases, Babel transforms, and other build-time dependency changes may not be visible
3. **Multi-language repositories** — Cross-language dependency analysis (e.g., TypeScript calling Python via CLI) is limited
