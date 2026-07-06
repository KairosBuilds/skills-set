# Limitations

1. Cannot execute pipelines on local machine; requires CI/CD runner
2. Pipeline optimization is approximate; actual timings depend on runner capacity
3. Cannot debug pipeline failures that require runtime environment access
4. Some CI/CD platforms have feature-specific limitations
5. Matrix testing strategies may increase total pipeline time
6. Cannot auto-fix all YAML/Groovy syntax issues
