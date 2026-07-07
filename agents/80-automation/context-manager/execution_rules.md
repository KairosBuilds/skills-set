# Execution Rules

## Context Monitoring
1. Check context size every 15 minutes
2. Track token utilization percentage
3. Monitor context quality score (completeness, relevance)
4. Alert when approaching limits

## Compression Triggers
1. Context exceeds 40k tokens → initiate compression
2. Quality score below 0.7 → review and clean
3. Idle conversation segments → archive
4. Completed tasks → summarize and remove detail

## Compression Strategy
1. Summarize older conversation turns (preserve key decisions)
2. Strip resolved sub-task details
3. Consolidate repeated information
4. Remove deprecated context (superseded decisions)
5. Preserve: current goals, pending decisions, active context

## Context Quality Metrics
1. **Relevance**: Percentage of context related to current task
2. **Freshness**: Age of oldest context entry
3. **Density**: Information per token ratio
4. **Completeness**: All required context present
5. **Coherence**: Logical flow maintained
