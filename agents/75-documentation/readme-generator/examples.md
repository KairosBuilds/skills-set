# Examples

## Basic README Generation
```bash
opencode readme-generator --project ./my-app
```

## With Custom Sections
```bash
opencode readme-generator --project ./my-app --sections "Title,Usage,API,License"
```

## With Badges
```bash
opencode readme-generator --project ./my-app --badges --ci github-actions --coverage codecov
```

## Output
Creates `README.md` in the project root with badges, installation instructions, usage examples, and contribution guidelines.
