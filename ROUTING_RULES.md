# Kairos AI — Routing Rules

## Routing Decision Tree

```
User Request
  ├── Contains "bug", "error", "crash", "exception"
  │   → Debugging category
  │
  ├── Contains "security", "vulnerability", "audit"
  │   → Security category
  │
  ├── Contains "performance", "slow", "optimize"
  │   → Performance/Optimization category
  │
  ├── Contains "test", "testing", "coverage"
  │   → Testing category
  │
  ├── Contains "documentation", "docs", "readme"
  │   → Documentation category
  │
  ├── Contains "deploy", "release", "ship"
  │   → Deployment/Release category
  │
  ├── Contains "architect", "design", "structure"
  │   → Architecture category
  │
  ├── Contains "review", "refactor"
  │   → Review category
  │
  ├── Contains "plan", "sprint", "roadmap"
  │   → Planning category
  │
  ├── Contains "research", "investigate"
  │   → Research category
  │
  ├── Contains "monitor", "observe", "log"
  │   → Monitoring category
  │
  ├── Contains "config", "setup", "init"
  │   → Automation category
  │
  ├── Contains "frontend", "ui", "react", "vue"
  │   → Frontend category
  │
  ├── Contains "backend", "api", "server"
  │   → Backend category
  │
  ├── Contains "mobile", "ios", "android"
  │   → Mobile category
  │
  ├── Contains "docker", "k8s", "ci/cd"
  │   → DevOps category
  │
  └── Default
      → Orchestrator (complex analysis)
```

## Cross-Category Routing
When a request spans multiple categories (e.g., "fix security bug in the React frontend"):
1. Orchestrator identifies all affected categories
2. Primary category processes first
3. Secondary categories process in dependency order
4. Orchestrator merges results

## Priority-Based Routing
- Critical priority agents execute first
- Blocking dependencies must complete before dependent tasks start
- Non-blocking tasks can run in parallel
- Low priority tasks queue behind higher priority work

## Conflict Resolution
If two agents could handle the same task:
1. Check agent priority (higher wins)
2. Check execution cost (lower cost preferred for equal priority)
3. Check confidence level (production > stable > experimental)
4. If still ambiguous, Orchestrator decides

## Agent Selection Algorithm
```
function select_agents(request):
    categories = classify(request)
    agents = []
    for category in categories:
        candidates = get_agents_in_category(category)
        for candidate in candidates:
            if matches_capability(candidate, request):
                score = calculate_score(candidate, request)
                agents.append((candidate, score))
    agents.sort_by(score, reverse=True)
    return agents[0:min(3, len(agents))]
```

## Fallback Routing
If the primary agent fails:
1. Try the secondary agent in the same category
2. Try a general-purpose agent
3. Escalate to Orchestrator
4. Orchestrator may re-route to a different category
