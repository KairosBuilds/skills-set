# Execution Rules

1. Always run terraform plan before apply; review proposed changes
2. Use remote state backends with state locking enabled
3. Tag all resources with environment, project, and owner tags
4. Use modules for reusable infrastructure components
5. Pin provider versions to avoid breaking changes
6. Never hardcode secrets; use variables or secret store
7. Separate configuration into root modules per environment
8. Run terraform validate and fmt before committing
