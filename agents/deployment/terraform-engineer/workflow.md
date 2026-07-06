# Workflow

1. **Analyze Requirements**: Determine cloud provider, resources needed
2. **Design Infrastructure**: Plan resource hierarchy, network topology
3. **Configure Backend**: Set up remote state storage (S3, GCS, Azure)
4. **Create Modules**: Develop reusable resource modules
5. **Define Resources**: Write HCL for compute, network, storage, IAM
6. **Configure Variables**: Define input variables with validation
7. **Generate Outputs**: Create useful output values
8. **Validate**: Run terraform validate, terraform fmt
9. **Plan**: Execute terraform plan and review changes
10. **Apply**: Deploy infrastructure with terraform apply
