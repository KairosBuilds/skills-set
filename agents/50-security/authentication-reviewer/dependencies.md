# Examples
`javascript
// ❌ JWT with none algorithm vulnerability
jwt.verify(token, null, { algorithms: ['none', 'HS256'] });

// ✅ JWT with explicit algorithm enforcement
jwt.verify(token, secret, { algorithms: ['HS256'] });
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\security\authentication-reviewer\examples.md" -Encoding UTF8

@"
# Dependencies
- security/hunt-auth-bypass (skill)
- security/hunt-oauth (skill)
- security/hunt-saml (skill)
- JWT Tool, SAML Raider, OAuth2 Proxy
