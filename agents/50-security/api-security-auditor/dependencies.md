# Examples
`python
# ❌ Mass assignment vulnerability
class UserAPI(Resource):
    def put(self, user_id):
        user = User.query.get(user_id)
        user.update(request.json)  # Can set is_admin=True

# ✅ Whitelist fields
allowed = ['name', 'email']
for key, value in request.json.items():
    if key in allowed:
        setattr(user, key, value)
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\security\api-security-auditor\examples.md" -Encoding UTF8

@"
# Dependencies
- security/hunt-api-misconfig (skill)
- security/hunt-graphql (skill)
- inql, graphql-editor, grpcurl, Postman, Burp Suite
