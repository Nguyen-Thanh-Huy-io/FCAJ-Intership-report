---
title : "Prerequisites"
date : 2024-01-01 
weight : 2 
chapter : false
pre : " <b> 5.2. </b> "
---

#### Technology stack
+ Frontend: React 18, Vite, React Router, MUI, Radix UI, Tailwind CSS.
+ Backend: Node.js, Express, Prisma, Socket.IO, BullMQ, Redis.
+ Infrastructure: AWS, Terraform, S3, CloudFront, ECS, ALB, RDS, ElastiCache, ECR, Route 53, Secrets Manager.
+ Deployment: GitHub Actions, Docker, environment-based staging setup.

#### What is needed to run the project
+ Node.js and npm or pnpm.
+ Docker for local services and container workflows.
+ AWS credentials for provisioning staging infrastructure.
+ A PostgreSQL/MySQL-compatible database is not required locally if you use the managed AWS stack.

{{% notice warning %}}
NEED AN IMAGE + setup flow showing developer machine, Docker, AWS account, Terraform, and the staging deployment pipeline.
{{% /notice %}}

{{< img "images/5-Workshop/5.2-Prerequisite/create-stack1.png" "create stack" >}}

#### Project setup in one view
+ Install dependencies for frontend and backend.
+ Configure environment variables for API, database, Redis, and social integrations.
+ Provision AWS staging resources through Terraform.
+ Start the frontend and backend services.
+ Verify login, dashboard access, and external integrations.