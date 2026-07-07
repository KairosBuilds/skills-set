# Edge Case Analyzer — Examples

## Example 1: String Processing Function
**Function:** `splitAndCapitalize(input: string): string[]`
**Edge Cases:**
- Empty string `""` → should return `[]`
- Single character `"a"` → should return `["A"]`
- Only delimiters `",,"` → should skip empty tokens
- Unicode characters `"café"` → preserve accents
- Very long string (10MB+) → memory consideration
- Mixed whitespace `"a b  c"` → normalize spacing

## Example 2: Number Processing
**Function:** `calculateAverage(values: number[]): number`
**Edge Cases:**
- Empty array → define behavior (0 or error?)
- Single element → returns that element
- Negative numbers → still valid
- Floating point precision → rounding strategy
- NaN or Infinity values → filter or propagate?
- Integer overflow → use safe math

## Example 3: API Request Handler
**Endpoint:** `POST /api/users`
**Edge Cases:**
- Missing body → 400 Bad Request
- Empty name field → validation error
- Duplicate email → conflict handling
- Special characters in name → XSS prevention
- Maximum field length → truncation vs rejection
- SQL injection attempts → parameterized queries
