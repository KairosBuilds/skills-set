# Examples

## Example 1: Extract Method
`python
# Before
def process(data):
    validate(data)
    price = calculate(data)
    tax = price * 0.08
    total = price + tax
    return total

# After
def process(data):
    validate(data)
    return calculate_total(data)

def calculate_total(data):
    price = calculate(data)
    tax = price * 0.08
    return price + tax
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\review\refactoring-agent\examples.md" -Encoding UTF8

@"
# Dependencies

## Internal Dependencies
- code-quality/code-reviewer (skill)
- testing/test-master (skill)

## External Tools
- ESLint with fix mode
- Prettier
- jscpd (copy-paste detection)
- TypeScript compiler (behavior preservation check)
- pytest/vitest (test runner)

## Runtime
- Node.js >= 18
- Python >= 3.10
