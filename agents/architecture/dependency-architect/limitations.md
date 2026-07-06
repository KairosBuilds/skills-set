# Dependency Architect Limitations

## Analysis Limitations

1. **Static analysis only** — Cannot detect runtime or dynamic dependencies
2. **No performance analysis** — Dependency size and bundle impact analysis is limited
3. **No transitive dependency resolution** — Deep transitive dependency trees may require package manager execution
4. **No license compliance** — Can identify dependencies but not perform full license compliance analysis

## Scope Limitations

1. **Not a package manager** — Does not install or update packages
2. **No vulnerability scanning** — Security vulnerabilities in dependencies are outside scope
3. **No build system design** — Build pipeline configuration is delegated to devops
4. **Limited to code dependencies** — Infrastructure, CI/CD, and operational dependencies are out of scope

## Knowledge Limitations

1. **Package ecosystem changes** — New package versions and ecosystem changes may not be fully reflected
2. **Vulnerability database** — Requires integration with vulnerability databases for CVE data
3. **Specific framework dependency quirks** — Framework-specific dependency resolution nuances may require specialist escalation
