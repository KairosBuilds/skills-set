# Execution Rules
1. Verify OAuth2 state parameter and PKCE usage
2. Check redirect URI validation against open redirects
3. Verify JWT algorithm enforcement (reject none, validate signature)
4. Check SAML assertion signature verification
5. Validate session management (fixation, timeout, invalidation)
6. Review MFA implementation for bypass vectors
7. Check password policy against best practices
