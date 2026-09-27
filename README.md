# Day 25 - Terraform Variables & Outputs

## Overview

This project demonstrates Terraform variables and outputs using the local provider.

## Technologies

- Terraform
- HCL
- WSL Ubuntu
- Git/GitHub

## What I Practiced

- Defining variables in `variables.tf`
- Referencing variables with `var.message`
- Overriding variables with `terraform apply -var='message=...'`
- Defining outputs in `outputs.tf`
- Reading outputs with `terraform output`
- Using `terraform plan` to verify infrastructure state
- Restoring the default configuration after a temporary variable override

## Project Structure

```
day25-terraform/
├── main.tf
├── variables.tf
├── outputs.tf
├── .gitignore
└── README.md
```

## Terraform Workflow

```bash
terraform init
terraform plan
terraform apply
terraform output
terraform destroy
```

## Key Learning

- **Variable** = input to Terraform
- **Output** = useful information returned by Terraform
- `var.message` reads the value of the `message` variable
- `-var` temporarily overrides a variable for a Terraform command
- Terraform plan can identify differences between configuration and managed state

## Security

Terraform state files and the `.terraform/` directory are excluded from Git. Credentials, tokens, private keys, and other secrets must never be committed.

## Author

Bilal - Cloud/DevOps learning journey
