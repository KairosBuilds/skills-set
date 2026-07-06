# Execution Rules

1. Use official base images with specific version tags, never latest
2. Implement multi-stage builds for smaller final images
3. Run containers as non-root user
4. Scan images for known vulnerabilities before deployment
5. Minimize layer count by combining RUN commands
6. Use .dockerignore to exclude unnecessary files
7. Label images with metadata (version, maintainer, build-date)
8. Never store secrets in Dockerfiles or environment files
