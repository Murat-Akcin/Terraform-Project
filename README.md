# Terraform-Project

![image](https://github.com/user-attachments/assets/e4bd9d00-5de2-4c77-acf4-e7befb4b9dd3)


This Terraform project sets up a complete AWS infrastructure with a modular, production-ready architecture. It includes a fully-featured VPC, public and private subnets, NAT gateway, multiple route tables, and an EC2 instance with IAM roles.

## 🌐 Key Features

- Modular VPC with public, private, database, Lambda, and EKS subnets
- NAT Gateway for outbound internet access in private subnets
- Route tables and ACLs for subnet isolation
- EC2 instance with IAM instance profile and security group
- EIP and SSM Parameter support
- IAM role and policy attachments for secure access
- Uses `data` sources for AWS region and identity

## 🧱 Modules

- `core_vpc`: VPC, subnets, route tables, ACLs, gateways
- `ec2-instance-bootcamp`: Launches EC2 with IAM, EIP, SSM

## 🔧 Requirements

- Terraform CLI >= 1.0
- AWS CLI configured (`aws configure`)
- AWS IAM user with permissions to create infrastructure

## 🚀 Usage

```bash
terraform init
terraform plan
terraform apply


🧹 Cleanup
bash
terraform destroy
