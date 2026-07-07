# Logic Error Detector — Workflow

1. **Input Reception**
   - Code with description of expected vs actual behavior
   - Function signatures and intended semantics

2. **Execution Path Tracing**
   - Trace all possible execution paths mentally
   - Identify branches and conditional logic
   - Map data transformations through the code

3. **Invariant Checking**
   - Identify implicit invariants
   - Check if invariants hold across all paths
   - Flag invariant violations

4. **Boundary Analysis**
   - Check loop bounds and termination conditions
   - Verify off-by-one handling
   - Validate comparison operators

5. **Algorithm Verification**
   - Compare implementation against intended algorithm
   - Identify missing steps or incorrect transformations
   - Check sorting, searching, and math operations

6. **Report**
   - Location of logic error
   - Expected vs actual behavior
   - Corrected logic with explanation
