---
title : "Cleanup"
date : 2024-01-01
weight : 5
chapter : false
pre : " <b> 5.5. </b> "
---

Congratulations on reaching the final part of the presentation.

#### What to clean up
+ Run Terraform destroy in the staging environment to remove the AWS resources managed by this project.
+ Remove the ECS service, ALB, RDS, ElastiCache, ECR, S3/CloudFront, Route 53, Secrets Manager, and related IAM resources from the stack.
+ If you created a separate state backend or bootstrap resources, remove those only after the main stack is gone.

#### Recommended Terraform cleanup flow
+ `terraform init`
+ `terraform destroy`
+ Review the plan carefully before confirming the destroy action.

{{% notice warning %}}
NEED AN IMAGE + cleanup slide showing Terraform destroy removing the AWS stack and returning the account to a clean state.
{{% /notice %}}

{{< img "images/5-Workshop/5.5-Policy/s3-bucket-policy.png" "endpoint diagram" >}}

#### Closing note
Thank you for reading the presentation. The project can be removed cleanly with Terraform once you finish the demo or validation.


