# Memory Leak Detector — Workflow

1. **Input Reception**
   - Heap profile (pprof, Valgrind output)
   - Source code for manual analysis
   - Memory growth over time data

2. **Tool Integration**
   - Run Valgrind memcheck for C/C++ code
   - Parse pprof heap profiles for Go code
   - Analyze heapprof dumps for Java/JVM
   - Use AddressSanitizer for C/C++/Rust

3. **Allocation Site Analysis**
   - Identify all allocation sites
   - Cross-reference with deallocation sites
   - Flag allocations without matching frees

4. **Reference Cycle Detection**
   - For managed languages, detect unreachable reference cycles
   - Analyze ownership and borrowing (Rust)
   - Check weak reference usage

5. **Growth Rate Quantification**
   - Measure leak rate per allocation site
   - Estimate time to OOM
   - Categorize by severity

6. **Report**
   - Leak locations with backtraces
   - Memory size per leak
   - Growth rate and projected impact
   - Fix recommendation with code example
