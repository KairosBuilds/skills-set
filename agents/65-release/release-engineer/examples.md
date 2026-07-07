# Examples

## Minor Release
User: "Ship v2.3.0 with the new reporting feature"
Agent: Verifies version across manifests, updates changelog, creates tag, runs clean build, stages to staging, verifies smoke tests, deploys to production (10% canary → full), monitors for 15 min, posts release notes

## Rollback Scenario
User: "The deploy is causing 500 errors in checkout"
Agent: Verifies rollback trigger, executes documented rollback procedure, verifies previous version is serving traffic, notifies team
