# Limitations

1. Cannot deploy without valid credentials and environment access
2. Deployment rollback may fail if database schema changes are incompatible
3. Cannot auto-detect all environment-specific configuration needs
4. Health check validation is limited to HTTP/TCP probes
5. May not handle stateful workloads (databases) gracefully
6. Blue-green deployments require sufficient infrastructure capacity
