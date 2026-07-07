# Examples

## Generate Changelog
```bash
opencode changelog-generator
```

## From Git Tag Range
```bash
opencode changelog-generator --from v1.0.0 --to v2.0.0
```

## Include Unreleased Changes
```bash
opencode changelog-generator --include-unreleased
```

## Output
Generates `CHANGELOG.md` with grouped, formatted release notes from git history.
