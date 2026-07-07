# Execution Rules

## Gate Enforcement
1. All quality gates must pass before promotion to next environment
2. Security scan failures are blocking — escalate immediately
3. Test coverage must not decrease from baseline
4. Typecheck and lint must pass without warnings

## Rollback Protocol
1. Detect failure within 60s of deployment
2. Auto-rollback staging; require manual approval for production
3. Log rollback reason and duration
4. Notify all stakeholders via configured channels

## Hotfix Handling
1. Hotfixes bypass minor/major gates but require security scan
2. Tag with `hotfix-` prefix
3. Merge back to develop branch after deployment

## Versioning
1. Follow semantic versioning (MAJOR.MINOR.PATCH)
2. Auto-increment PATCH for fixes, MINOR for features, MAJOR for breaking
3. Use semantic-version-manager for version calculations
