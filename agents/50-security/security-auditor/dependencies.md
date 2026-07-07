# Examples
`python
# ❌ SQL Injection vulnerability
query = f"SELECT * FROM users WHERE email = '{email}'"

# ✅ Parameterized query
query = "SELECT * FROM users WHERE email = %s"
cursor.execute(query, (email,))
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\security\security-auditor\examples.md" -Encoding UTF8

@"
# Dependencies
- security/security-reviewer (skill)
- security/secure-code-guardian (skill)
- Bandit, Safety, npm audit, Trivy, OWASP ZAP
