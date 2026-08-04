---
title : "CI/CD Pipeline"
date : 2024-01-01
weight : 4
chapter : false
pre : " <b> 5.4. </b> "
---

#### Terraform module for delivery automation

This chapter explains how the repository automates release delivery through CodeStar, CodeBuild, and CodePipeline.

#### CI/CD services created by Terraform
+ S3 bucket for pipeline artifacts.
+ CodeStar connection for GitHub source access.
+ IAM roles and policies for CodePipeline and CodeBuild.
+ CodeBuild projects for backend and frontend builds.
+ CodePipelines for backend and frontend release stages.

#### Build behavior
+ Backend build runs in privileged Docker mode because it builds container images.
+ Frontend build publishes assets to the S3 bucket and invalidates CloudFront.
+ Both pipelines source from the same GitHub branch configured in Terraform.

{{% notice warning %}}
NEED AN IMAGE + CI/CD architecture showing GitHub, CodeStar connection, CodeBuild, CodePipeline, S3 artifacts, ECR, ECS, and CloudFront.
{{% /notice %}}

{{< img "images/5-Workshop/5.4-S3-onprem/diagram3.png" "Interface endpoint architecture" >}}

#### Why this matters
+ Releases are reproducible and tied to source control.
+ Build logic is separated from application code.
+ The same Terraform stack defines the delivery path for both frontend and backend.



