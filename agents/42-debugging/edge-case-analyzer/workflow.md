# Edge Case Analyzer — Workflow

1. **Input Reception**
   - Function signature with parameter types
   - Code with conditional logic
   - API contract or interface definition

2. **Input Domain Mapping**
   - Map all input parameters and their domains
   - Identify type boundaries (integer min/max, string length, etc.)
   - Document implicit constraints

3. **Boundary Value Enumeration**
   - Empty collections and strings
   - Null values
   - Minimum and maximum values
   - Negative numbers where positive expected
   - Zero values
   - Special values (NaN, Infinity, etc.)
   - Unicode and special characters for strings

4. **State Transition Analysis**
   - Identify state machines in the code
   - List all valid state transitions
   - Check invalid or unexpected transitions

5. **Combinatorial Consideration**
   - Identify interactions between parameters
   - Prioritize realistic edge case combinations
   - Flag security-relevant combinations

6. **Report**
   - Prioritized list of edge cases
   - Expected behavior for each
   - Suggested test cases
   - Severity and risk rating
