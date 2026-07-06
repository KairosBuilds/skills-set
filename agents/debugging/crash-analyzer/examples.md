# Crash Analyzer — Examples

## Example 1: NullReferenceException (.NET)
**Input Stack Trace:**
```
at MyApp.Services.OrderProcessor.CalculateTotal()
at MyApp.Controllers.OrderController.Submit()
NullReferenceException: Object reference not set to instance
```
**Analysis:** `_taxCalculator` field was not initialized in constructor
**Crash Type:** Null pointer dereference
**Root Cause:** Missing dependency initialization

## Example 2: Segmentation Fault (C++)
**Input:** Core dump signal SIGSEGV
**Faulting Address:** 0x0
**Analysis:** Dereferencing a dangling pointer after object destruction
**Crash Type:** Use-after-free
**Root Cause:** Object lifetime mismatch

## Example 3: IndexOutOfBoundsException (Java)
**Input Stack Trace:**
```
java.lang.IndexOutOfBoundsException: Index 10 out of bounds for length 10
    at MyApp.Utils.CacheManager.get()
```
**Analysis:** List index starts at 0, but code accesses `list.size()` directly
**Root Cause:** Off-by-one in list access
