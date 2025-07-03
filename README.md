# Terraform AWS VPC Setup

This project provisions a basic AWS VPC infrastructure using Terraform. It includes a VPC, public and private subnets, an internet gateway, a NAT gateway, and route tables for public and private networking.

## Files
- `vpc.tf`: Main VPC, subnets, gateways, and route tables
- `variables.tf`: Input variables (e.g., availability zone)
- `terraform.tfvars`: Variable values (not committed, see `.gitignore`)
- `providers.tf`: Provider configuration
- `sg.tf`: Security groups
- `key.tf`: Key pair resources
- `output.tf`: Output values

## Usage
1. Initialize Terraform:
   ```bash
   terraform init
   ```
2. Review and apply the plan:
   ```bash
   terraform plan
   terraform apply
   ```
3. Destroy resources when done:
   ```bash
   terraform destroy
   ```

## Prerequisites
- [Terraform](https://www.terraform.io/downloads.html)
- AWS credentials configured (via environment variables or AWS CLI)

## Notes
- Sensitive files like `terraform.tfvars` are excluded from version control (see `.gitignore`).
- Edit `variables.tf` and `terraform.tfvars` to customize your deployment.

## License
MIT License
