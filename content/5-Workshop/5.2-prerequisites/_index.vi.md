---
title : "Điều kiện cần"
date : 2024-01-01 
weight : 2
chapter : false
pre : " <b> 5.2. </b> "
---

#### Công nghệ sử dụng
+ Frontend: React 18, Vite, React Router, MUI, Radix UI, Tailwind CSS.
+ Backend: Node.js, Express, Prisma, Socket.IO, BullMQ, Redis.
+ Hạ tầng: AWS, Terraform, S3, CloudFront, ECS, ALB, RDS, ElastiCache, ECR, Route 53, Secrets Manager.
+ Triển khai: GitHub Actions, Docker, môi trường staging theo biến cấu hình.

#### Cần chuẩn bị gì
+ Node.js và npm hoặc pnpm.
+ Docker để chạy dịch vụ cục bộ và các luồng container.
+ AWS credentials để triển khai hạ tầng staging.
+ Không cần chạy database local nếu dùng toàn bộ stack trên AWS.

{{% notice warning %}}
NEED AN IMAGE + luồng chuẩn bị hệ thống thể hiện máy lập trình, Docker, AWS account, Terraform và pipeline triển khai staging.
{{% /notice %}}

{{< img "images/5-Workshop/5.2-Prerequisite/create-stack1.png" "create stack" >}}

#### Quy trình setup ngắn gọn
+ Cài dependency cho frontend và backend.
+ Cấu hình biến môi trường cho API, database, Redis và các tích hợp mạng xã hội.
+ Provision hạ tầng AWS staging bằng Terraform.
+ Khởi động frontend và backend.
+ Kiểm tra đăng nhập, dashboard và các tích hợp ngoài.