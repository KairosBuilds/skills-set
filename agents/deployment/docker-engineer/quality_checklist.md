# Quality Checklist

- [ ] Base image uses specific version tag (not latest)
- [ ] Multi-stage builds are used to minimize image size
- [ ] Container runs as non-root user
- [ ] .dockerignore file exists
- [ ] Vulnerabilities are scanned and addressed
- [ ] Image labels include metadata
- [ ] No secrets in Dockerfile or environment files
- [ ] EXPOSE directives match actual application ports
- [ ] HEALTHCHECK instruction is present
- [ ] Resource limits are configured in Compose
