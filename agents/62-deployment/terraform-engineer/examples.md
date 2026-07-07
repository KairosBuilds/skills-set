# Examples

## Initialize Terraform Project
```bash
opencode terraform-engineer init --provider aws --region us-east-1
```

## Create VPC Module
```bash
opencode terraform-engineer create module --name vpc --resources vpc,subnets,igw
```

## Plan Infrastructure
```bash
opencode terraform-engineer plan --env staging
```

## Output
Creates Terraform configurations for cloud infrastructure provisioning with modules, variables, and remote state management.
