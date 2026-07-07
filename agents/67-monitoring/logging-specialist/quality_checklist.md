# Quality Checklist

## Setup
- [ ] Log schema defined with required fields
- [ ] Log levels configured per environment
- [ ] Log shipping pipeline tested
- [ ] Retention policy configured
- [ ] Rotation and archival configured
- [ ] Performance benchmarked (<5% overhead)

## Configuration
- [ ] No sensitive data in log fields
- [ ] Error logs include stack traces
- [ ] Request tracing headers included
- [ ] Service name and environment correct
- [ ] Sampling rate appropriate for volume

## Monitoring
- [ ] Log shipping health monitored
- [ ] Disk space alerts configured
- [ ] Error rate alerts set up
- [ ] Log index management automated
- [ ] Dashboards created for key metrics
