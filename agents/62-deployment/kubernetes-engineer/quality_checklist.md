# Quality Checklist

- [ ] All containers have resource requests and limits
- [ ] Liveness and readiness probes are configured
- [ ] Pod security context enforces non-root
- [ ] RBAC follows least-privilege principle
- [ ] NetworkPolicies are defined for each namespace
- [ ] Secrets are not exposed in environment variables
- [ ] ConfigMaps are used for non-sensitive configuration
- [ ] Deployments have appropriate replica counts
- [ ] Service types match access requirements
- [ ] Helm charts have values.yaml schema
