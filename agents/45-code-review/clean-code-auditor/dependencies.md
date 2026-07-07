# Examples
`python
# ❌ Magic number, unclear name
def calc(x):
    return x * 0.08

# ✅ Named constant, descriptive name
TAX_RATE = 0.08
def calculate_tax(amount):
    return amount * TAX_RATE
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\review\clean-code-auditor\examples.md" -Encoding UTF8

@"
# Dependencies
- code-quality/code-reviewer (skill)
