# Bug Finder — Workflow

1. **Input Reception**
   - Source code files, snippets, or repository paths
   - Optional: bug description, error logs, expected behavior

2. **Static Analysis**
   - Parse AST and identify code structure
   - Apply pattern matching for known bug signatures
   - Run taint tracking for security-relevant bugs
   - Execute data flow analysis for state-related bugs

3. **Cross-Reference**
   - Compare against bug pattern database
   - Filter false positives through heuristic rules
   - Rank findings by severity and confidence

4. **Contextual Analysis**
   - Check surrounding code for related issues
   - Verify bug reproducibility conditions
   - Assess potential impact

5. **Report Generation**
   - Output structured report with:
   - File path and line numbers
   - Bug type and severity classification
   - Description of the issue
   - Suggested reproduction steps
   - Confidence score

6. **Handoff**
   - Pass findings to Bug Fixer agent
   - Include all context for efficient fixing
