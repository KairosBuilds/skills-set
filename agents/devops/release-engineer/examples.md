# Examples

## Create Release
```bash
opencode release-engineer create --version 2.1.0 --branch main
```

## Generate Release Notes
```bash
opencode release-engineer notes --from v2.0.0 --to v2.1.0
```

## Promote Artifact
```bash
opencode release-engineer promote --artifact my-app-2.1.0.jar --stage prod
```

## Output
Manages the complete release lifecycle including versioning, artifact management, and deployment coordination.
