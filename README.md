# Terraform AWS 3-Tier DevOps Project

## Overview
This project demonstrates how to provision and manage a production-ready
3-tier AWS architecture using Terraform with DevOps best practices.

## Architecture
- VPC with public & private subnets
- EC2 + Auto Scaling Group
- Application Load Balancer
- Secure networking (Security Groups)
- Remote Terraform state (S3 + DynamoDB)

## DevOps Practices Implemented
- Infrastructure as Code (Terraform)
- Modular Terraform design
- CI pipeline for validation and planning
- CD pipeline with manual approval for production
- Environment separation (dev / prod)
- Secure secrets management (GitHub Secrets)
- Manual destroy protection

## CI/CD Workflow
- Pull Request → terraform fmt / validate / plan
- Merge to main → manual approval → terraform apply

## How to Run
```bash
cd environments/dev
terraform init
terraform plan
terraform apply
