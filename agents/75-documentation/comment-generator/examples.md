# Examples

## Add Comments to Complex Code
```bash
opencode comment-generator --path ./src --style line
```

## Generate Docstrings Only
```bash
opencode comment-generator --path ./src --style docstrings --format jsdoc
```

## Focus on High-Complexity Functions
```bash
opencode comment-generator --path ./src --min-complexity 5
```

## Output
Adds meaningful comments and docstrings to source code, focusing on non-obvious logic and complex sections.
