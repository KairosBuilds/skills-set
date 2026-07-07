# Execution Rules
1. Check every endpoint for authorization enforcement
2. Test for IDOR in all resource-access endpoints
3. Verify role hierarchy doesn't allow privilege escalation
4. Check for missing authorization in admin endpoints
5. Validate default-deny principle is followed
6. Test horizontal access control between users
7. Check API-level authorization (not just UI hiding)
