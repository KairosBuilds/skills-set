# Workflow

1. **Parse Manifests**: Read package.json, requirements.txt, Cargo.toml, etc.
2. **Build Tree**: Resolve full transitive dependency graph
3. **Version Check**: Compare versions against latest releases
4. **Vulnerability Scan**: Query OSV/npm audit for CVEs
5. **License Analysis**: Verify each dependency license
6. **Conflict Detection**: Find version mismatches
7. **Optimize**: Suggest removals, dedup, or replacements
8. **Report**: Generate dependency health report
