# Cloud Architect Examples

## Example 1: AWS Migration

**Request:** "Migrate our on-premise application to AWS"

**Output:**
- Assessment: 12 servers, 3-tier Java app, Oracle database
- Strategy: Rehost (Lift & Shift) initially, then Replatform (RDS for Oracle)
- Architecture: EC2 Auto Scaling groups, ALB, RDS Multi-AZ, S3 for static assets
- Migration: 5 waves over 3 months, database replicated via DMS
- Cost: Estimated 35% savings compared to on-premise over 3 years
- DR: Cross-region replication, RPO 15min, RTO 4hr

## Example 2: Multi-Cloud Design

**Request:** "Design a multi-cloud architecture for high availability"

**Output:**
- Primary: AWS us-east-1
- Secondary: GCP us-central1
- DNS: Global traffic management via Cloudflare
- Data: Active-active with conflict resolution, read replicas in each region
- Failover: Automated health checks, DNS failover under 60s
- Cost: 25-40% premium over single-cloud; justified by 99.999% availability requirement

## Example 3: Cost Optimization Review

**Request:** "Our AWS bill is $50K/month. Where can we save?"

**Analysis:**
- Finding: 40% of EC2 instances are idle on weekends (savings: schedule start/stop)
- Finding: No reserved instances for steady-state workloads (savings: 30% with 1-year RIs)
- Finding: Unused EBS volumes and old snapshots (savings: $2K/month)
- Finding: Data transfer costs high from cross-AZ traffic (savings: colocate services)
- Total estimated savings: $12K/month (24%)
