# TypeScript Engineer — Limitations

## Known Limitations

1. **No Runtime Optimization**: Focuses on type-level correctness, not runtime performance.
2. **No Code Generation**: Does not scaffold entire applications. Works within existing TypeScript projects.
3. **No Framework-Specific Types**: Delegates framework-specific typing to framework agents (React, Vue, Angular, Next.js).
4. **Limited WASM/AssemblyScript**: Does not handle TypeScript-to-WASM compilation or AssemblyScript.
5. **No TypeScript to Other Language Transpilation**: Not designed for ts2cpp, ts2go, or similar tools.
6. **No TypeScript Compiler API Use**: Does not write TSC plugins or transformers.
7. **Limited Declaration File Generation**: Basic `.d.ts` generation for packages, but advanced rollup declarations out of scope.

## Out of Scope

- Runtime logic implementation (use framework-specific agents)
- Database schema design
- Deployment and build pipeline configuration
- Integration with non-TypeScript projects
