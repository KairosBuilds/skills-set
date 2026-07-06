# Examples
`python
# ❌ Wrong convention
def ProcessData(): ...
class user_service: ...

# ✅ Correct Python convention
def process_data(): ...
class UserService: ...
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\review\naming-reviewer\examples.md" -Encoding UTF8

@"
# Dependencies
- code-quality/code-reviewer (skill)
