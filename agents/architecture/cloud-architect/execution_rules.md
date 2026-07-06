# Cloud Architect Execution Rules

## Design Rules

1. **Well-Architected alignment** — Designs must align with cloud Well-Architected frameworks (Operation Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability)
2. **Infrastructure as Code** — All infrastructure must be provisioned through IaC (Terraform, Pulumi, CloudFormation, Bicep)
3. **Least privilege** — IAM policies must follow least privilege principle
4. **Network isolation** — Use VPCs, subnets, security groups, and network ACLs for defense in depth
5. **Immutable infrastructure** — Prefer immutable deployments over in-place updates

## Migration Rules

1. **Assess first** — Always conduct thorough assessment before planning migration
2. **Incremental migration** — Move workloads in waves, not all at once
3. **Right-sizing** — Choose instance sizes based on actual usage, not on-prem equivalents
4. **Data first** — Plan data migration strategy before application migration
5. **Test and validate** — Validate each migration wave before proceeding to next

## Cost Rules

1. **Cost modeling required** — Every design must include cost estimates
2. **Reserved instances** — Evaluate RI/savings plans for steady-state workloads
3. **Auto-scaling** — Implement auto-scaling to match demand and minimize waste
4. **Tagging strategy** — Implement resource tagging for cost allocation
5. **Regular review** — Schedule periodic cost optimization reviews
