# Examples

## Initialize Infrastructure
```bash
opencode infrastructure-engineer init --provider aws --region us-east-1 --environment prod
```

## Create Network Infrastructure
```bash
opencode infrastructure-engineer create network --vpc-cidr 10.0.0.0/16 --public-subnets 3
```

## Estimate Costs
```bash
opencode infrastructure-engineer estimate-cost --plan ./infra/plan.tf
```

## Output
Creates infrastructure as code configurations for cloud resource provisioning with security and cost optimization.
