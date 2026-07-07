# Examples

## Create GitHub Actions Pipeline
```bash
opencode cicd-engineer init --type github-actions --project ./my-app
```

## Create Jenkins Pipeline
```bash
opencode cicd-engineer init --type jenkins --project ./my-app
```

## Add Security Scanning
```bash
opencode cicd-engineer add-scan --type sast --tool semgrep
```

## Output
Creates CI/CD pipeline configuration files for automated build, test, and deployment workflows.
