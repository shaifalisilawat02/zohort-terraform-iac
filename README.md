# zohort-terraform-iac

This Terraform configuration provisions an **AWS S3 bucket** with the following settings:

- Bucket name: `zohort-devops-shaifali`
- Versioning enabled
- Public access blocked

This repository provisions an **AWS S3 bucket** using Terraform, following enterprise best practices.

## Features
- Creates an S3 bucket with versioning enabled
- Blocks all public access
- Outputs the bucket name after deployment
- Uses S3 remote backend and DynamoDB for state management

## Prerequisites
- Terraform installed (>= 1.3.0)
- AWS CLI configured with valid credentials
- Remote backend S3 bucket & DynamoDB table already created (for state & locking)

## Steps to Deploy

1. Clone the repo:
   ```bash
   git clone https://github.com/shaifalisilawat02/zohort-terraform-iac.git
   cd zohort-terraform-iac
   ```

2. Initialize Terraform:
   ```bash
   terraform init
   ```

3. Preview the plan:
   ```bash
   terraform plan
   ```

4. Apply the configuration:
   ```bash
   terraform apply
   ```

5. Type `yes` when prompted to confirm.

6. After apply, you will see the bucket name output. Example:
   ```text
   Apply complete! Resources: 1 added, 0 changed, 0 destroyed.

   Outputs:

   bucket_name = "zohort-devops-shaifali"
   ```

7. Clean up — to destroy the bucket:
   ```bash
   terraform destroy
   ```
