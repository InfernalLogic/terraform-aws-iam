# IAM assumable roles with SAML Identity Provider example

Configuration in this directory creates several IAM roles which can be assumed by users with a SAML Identity Provider.

# Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

Run `terraform destroy` when you don't need these resources.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.12.6 |
| aws | >= 2.23 |

## Providers

| Name | Version |
|------|---------|
| aws | >= 2.23 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| iam_assumable_roles_with_saml | ../../modules/iam-assumable-roles-with-saml |  |
| iam_assumable_roles_with_saml_custom | ../../modules/iam-assumable-roles-with-saml |  |
| iam_assumable_roles_with_saml_second_provider | ../../modules/iam-assumable-roles-with-saml |  |

## Resources

| Name |
|------|
| [aws_iam_saml_provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_saml_provider) |

## Inputs

No input.

## Outputs

| Name | Description |
|------|-------------|
| admin\_iam\_role\_arn | ARN of admin IAM role |
| admin\_iam\_role\_name | Name of admin IAM role |
| admin\_iam\_role\_path | Path of admin IAM role |
| poweruser\_iam\_role\_arn | ARN of poweruser IAM role |
| poweruser\_iam\_role\_name | Name of poweruser IAM role |
| poweruser\_iam\_role\_path | Path of poweruser IAM role |
| readonly\_iam\_role\_arn | ARN of readonly IAM role |
| readonly\_iam\_role\_name | Name of readonly IAM role |
| readonly\_iam\_role\_path | Path of readonly IAM role |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
