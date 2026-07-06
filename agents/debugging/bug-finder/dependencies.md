# Bug Finder — Dependencies

## Internal Dependencies
- **Bug Fixer:** Receives findings for fix implementation
- **Stack Trace Analyzer:** Provides additional context for crash-related bugs

## Tool Dependencies
- AST Parser (language-specific)
- Pattern Database (built-in bug signatures)
- Taint Analysis Engine
- Data Flow Analyzer

## Runtime Dependencies
- Language runtime for the target code
- Source code access (filesystem or repository)
- No network access required for static analysis
