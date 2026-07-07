# Execution Rules

## Fix Prioritization
1. Safety-critical fixes first (security, data loss)
2. Build-breaking fixes second (lint, type, syntax)
3. Code quality fixes third (formatting, style)

## Edit Loop Detection
1. Track consecutive failed edit attempts
2. Threshold: 5 attempts triggers loop break
3. On loop break: analyze root cause, suggest new approach
4. Never retry same fix more than 3 times

## Merge Conflict Resolution
1. Analyze conflict markers
2. Understand both branches' intent
3. Apply safe merge strategy (theirs/ours/manual)
4. Verify build passes after resolution
5. Never silently discard changes

## Verification Gate
1. All auto-fixes must pass through verification-agent
2. Verify build, lint, typecheck after fix
3. Rollback if verification fails
4. Log fix attempts and success rate
