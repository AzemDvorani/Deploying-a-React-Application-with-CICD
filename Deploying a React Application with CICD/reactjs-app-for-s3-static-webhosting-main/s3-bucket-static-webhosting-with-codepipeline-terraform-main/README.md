## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.25.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_codebuild_project.codebuild](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/codebuild_project) | resource |
| [aws_codepipeline.codepipeline1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/codepipeline) | resource |
| [aws_iam_role.codebuild_role1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.codepipeline_role1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role_policy.codebuild_policy1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.codepipeline_policy1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_s3_bucket.app_bucket](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.pipeline_bucket](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket_policy.app_bucket_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_policy) | resource |
| [aws_s3_bucket_policy.pipeline_bucket_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_policy) | resource |
| [aws_caller_identity.current](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/caller_identity) | data source |
| [aws_codestarconnections_connection.github](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/codestarconnections_connection) | data source |
| [aws_region.current](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_access_key"></a> [access\_key](#input\_access\_key) | access key | `any` | n/a | yes |
| <a name="input_app_bucket_name"></a> [app\_bucket\_name](#input\_app\_bucket\_name) | app bucket name | `string` | `"easydeploy-test-638140"` | no |
| <a name="input_connection_arn"></a> [connection\_arn](#input\_connection\_arn) | Arn for the CodeStar Connection | `string` | n/a | yes |
| <a name="input_pipeline_bucket_name"></a> [pipeline\_bucket\_name](#input\_pipeline\_bucket\_name) | pipeline bucket name | `string` | `"test-638140"` | no |
| <a name="input_projectname"></a> [projectname](#input\_projectname) | pipeline project name | `string` | `"easydeploy"` | no |
| <a name="input_repo_branch_name"></a> [repo\_branch\_name](#input\_repo\_branch\_name) | github branch name | `string` | `"main"` | no |
| <a name="input_repo_id"></a> [repo\_id](#input\_repo\_id) | github repository id | `string` | `"easydeploy-cloud/reactjs-app-for-s3-static-webhosting"` | no |
| <a name="input_secret_key"></a> [secret\_key](#input\_secret\_key) | secret key | `any` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_static_website_endpoint"></a> [static\_website\_endpoint](#output\_static\_website\_endpoint) | static s3 application bucket endpoint |
