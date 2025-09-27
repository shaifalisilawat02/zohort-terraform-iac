# zohort-terraform-iac
This Terraform configuration provisions an **AWS S3 bucket** with the following settings:

- Bucket name: `zohort-devops-shaifali`
- Versioning enabled
- Public access blocked

## Prerequisites

- Terraform >= 1.5.0
- AWS CLI configured with proper credentials
- AWS account with permissions to create S3 buckets

## Steps to Deploy


```bash
git clone https://github.com/shaifalisilawat02/zohort-terraform-iac.git

Initialize Terraform:
terraform init


Preview the plan:
terraform plan


Apply the configuration:
terraform apply


Type yes when prompted.
After apply, you will see the bucket name output:
Apply complete! Resources: 1 added, 0 changed, 0 destroyed.

Outputs:
bucket_name = "zohort-devops-shaifali"

Clean Up
To destroy the bucket:
terraform destroy

terraform destroy
