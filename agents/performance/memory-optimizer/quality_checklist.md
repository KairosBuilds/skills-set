# Quality Checklist

- [ ] Heap snapshots collected at two time points
- [ ] Snapshot diff identifies growing objects
- [ ] Retention paths traced to root cause
- [ ] Leak is reproduced consistently
- [ ] Fix applied and verified with new snapshot
- [ ] Soak test confirms stable memory usage
- [ ] GC pressure measured (frequency, pause time)
- [ ] Large object graphs analyzed for waste
- [ ] Memory budget set for critical components
- [ ] Monitoring alerts on memory growth trends
