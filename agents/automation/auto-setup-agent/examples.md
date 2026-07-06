# Examples

## Example 1: Standard Setup
```
Input: "Set up the project for development"
Actions:
1. Read README.md (npm install, npm run dev)
2. Detect package.json → Node.js project
3. Check Node version (v18 → OK)
4. Run npm install (all 152 packages)
5. Run npm run build (success)
6. Run npm test (42 passing)
7. Setup complete ✓
```

## Example 2: Version Mismatch
```
Input: "Project setup fails with node version error"
Diagnosis:
- Project requires Node 20+
- Current Node: v16.14.0
- Fix: Install Node 20 via nvm
- nvm install 20; nvm use 20
- npm install → success
```

## Example 3: Missing Build Tools
```
Input: "Python project setup fails"
Diagnosis:
- pyproject.toml detected
- Python 3.11 installed ✓
- pip install fails - missing build tools
- Fix: pip install setuptools wheel
- pip install -e . → success
- pytest → 87 passing
```
