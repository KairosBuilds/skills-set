# Execution Rules
1. Scan entire git history, not just current state
2. Use entropy detection for non-pattern secrets
3. Verify findings to minimize false positives
4. Never log, display, or store discovered secrets in reports
5. Mask secrets in all output (show only first 4 chars)
6. Prioritize confirmed secrets over potential matches
7. Check for secrets in commit messages and PR descriptions
