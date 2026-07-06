# Quality Checklist

## Instrumentation
- [ ] All public endpoints instrumented
- [ ] Database calls have spans
- [ ] External service calls traced
- [ ] Background jobs instrumented
- [ ] Span naming follows convention
- [ ] Required attributes set on all spans

## Configuration
- [ ] Sampling strategy appropriate
- [ ] Error traces fully sampled
- [ ] Export interval configured
- [ ] Batch processing configured
- [ ] Collector pipeline healthy

## Correlation
- [ ] Logs include trace_id
- [ ] Metrics include service labels
- [ ] Distributed context propagated
- [ ] Headers propagated across services
- [ ] Trace → log → metric links work
