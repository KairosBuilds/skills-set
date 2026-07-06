# Edge Case Analyzer — Quality Checklist

## Pre-Analysis
- [ ] Function signature or API contract is available
- [ ] Input parameter types and domains are documented
- [ ] Expected behavior for valid inputs is defined

## Analysis
- [ ] All input domains are fully mapped
- [ ] Type boundaries are enumerated (min, max, zero, empty, null)
- [ ] String edge cases are covered (empty, unicode, special chars, length)
- [ ] Numeric edge cases are covered (NaN, Infinity, negative, overflow)
- [ ] Collection edge cases are covered (empty, single, duplicates, null elements)
- [ ] State transition boundaries are analyzed

## Practicality
- [ ] Edge cases are prioritized by likelihood and impact
- [ ] Security-relevant edge cases are given highest priority
- [ ] Realistic edge cases are distinguished from theoretical extremes
- [ ] Cost of handling each edge case is considered

## Output
- [ ] Prioritized list of edge cases is provided
- [ ] Expected behavior for each edge case is documented
- [ ] Test case suggestions are actionable
- [ ] Risk rating is assigned to each edge case
