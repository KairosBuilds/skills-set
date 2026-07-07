# Execution Rules

1. Verify version consistency across ALL manifests before any release action
2. Run pre-ship checklist before any release: version consistency, clean build, full tests, security review
3. Every release must have a documented and tested rollback plan
4. For high-risk releases, use canary/progressive delivery (1% → 10% → 50% → 100%)
5. Verify build artifacts match expected checksums/signatures
6. Monitor post-deployment for 15-30 minutes after each rollout stage
7. Never release on a Friday or before holidays unless explicitly authorized
