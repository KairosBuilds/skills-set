# Execution Rules

1. Run full regression suite before every release
2. Use selective regression based on affected modules
3. Never delete or skip existing regression tests
4. Flag new regressions immediately with detailed failure context
5. Maintain a known-good baseline for comparison
6. Prioritize critical path tests in every run
7. Keep regression suite execution under 30 minutes
8. Tag tests by risk level (critical, high, medium, low)
9. Archive regression reports for trend analysis
10. Automate regression triggers on merge to main
