# Race Condition Detector — Workflow

1. **Input Reception**
   - Source code with concurrent access patterns
   - Or: ThreadSanitizer output, execution trace

2. **Shared Memory Map**
   - Identify all shared mutable state
   - Map which threads access which variables
   - Classify access types (read, write, atomic)

3. **Synchronization Analysis**
   - Identify synchronization primitives (mutex, semaphore, channel)
   - Map lock coverage for each shared variable
   - Check lock ordering consistency
   - Verify atomic operation correctness

4. **Happens-Before Analysis**
   - Trace happens-before relationships
   - Identify conflicting access pairs without ordering
   - Distinguish benign vs harmful races

5. **Reproduction Strategy**
   - Determine timing conditions for race
   - Suggest stress testing approach
   - Provide minimal reproduction test

6. **Report**
   - Conflicting access pairs with locations
   - Thread and stack trace for each access
   - Fix recommendation (lock, atomic, channel)
