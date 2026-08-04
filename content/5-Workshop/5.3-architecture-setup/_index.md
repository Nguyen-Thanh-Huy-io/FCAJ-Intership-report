---
title : "Architecture and Setup"
date : 2024-01-01
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

#### AWS resources created by Terraform

This chapter presents the infrastructure that supports the application and how Terraform composes the stack.

#### Core AWS services
+ VPC with public and private subnets to separate traffic and workloads.
+ ALB in the public layer to receive web traffic.
+ ECS service and task definitions for the API and background workers.
+ RDS for the relational database and ElastiCache Redis for cache and queue support.
+ ECR for container images, S3 and CloudFront for the frontend, Route 53 for the domain, and Secrets Manager for runtime secrets.

#### Important properties
+ ECS service desired counts are set for one API and two worker tiers.
+ The database connection uses MySQL on port 3306.
+ Terraform injects environment variables and secret ARNs into the task definitions.
+ The frontend bucket is paired with CloudFront for public delivery.

{{% notice warning %}}
NEED AN IMAGE + overall architecture showing the VPC, ALB, ECS, RDS, Redis, ECR, S3/CloudFront, Route 53, and Secrets Manager.
{{% /notice %}}

{{< img "images/5-Workshop/5.3-S3-vpc/diagram2.png" "overview" >}}

#### Content

- [Infrastructure layout](5.3.1-infrastructure-layout/)
- [Resource properties](5.3.2-resource-properties/)