# Examples
`python
# ❌ IDOR — user can access any order
def get_order(order_id):
    return Order.objects.get(id=order_id)

# ✅ Owner check
def get_order(order_id, user):
    return Order.objects.get(id=order_id, user=user)
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\security\authorization-reviewer\examples.md" -Encoding UTF8

@"
# Dependencies
- security/hunt-idor (skill)
- Autorize (Burp), AuthZ tooling
