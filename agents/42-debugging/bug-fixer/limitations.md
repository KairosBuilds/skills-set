# Bug Fixer — Limitations

## Scope Limitations
- Cannot fix bugs without confirmed reproduction
- Complex multi-file fixes require manual review
- Cannot fix hardware or third-party API limitations
- Cannot migrate between major framework versions in a single fix

## Safety Limitations
- Always creates backup but large-scale changes need human review
- Cannot verify fixes in production — only in provided build/test environment
- Automated fix may not cover all edge cases
- Cannot fix security vulnerabilities requiring architectural changes

## Language-Specific Limitations
- Some language constructs (macros, metaprogramming) make safe fixes challenging
- Dynamically typed languages may have broader fix implications
- Generated code (protobuf, OpenAPI) should not be manually fixed
