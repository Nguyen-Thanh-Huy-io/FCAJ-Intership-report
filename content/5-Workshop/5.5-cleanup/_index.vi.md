---
title : "Dọn dẹp"
date : 2024-01-01
weight : 5
chapter : false
pre : " <b> 5.5 </b> "
---

Chúc mừng bạn đã đi đến phần cuối của bản trình bày.

#### Những gì cần dọn dẹp
+ Chạy Terraform destroy trong môi trường staging để xóa các tài nguyên AWS do dự án quản lý.
+ Xóa ECS service, ALB, RDS, ElastiCache, ECR, S3/CloudFront, Route 53, Secrets Manager và các IAM resources liên quan.
+ Nếu bạn tạo riêng state backend hoặc bootstrap resources, hãy xóa chúng sau khi stack chính đã được gỡ bỏ.

#### Luồng dọn dẹp bằng Terraform
+ `terraform init`
+ `terraform destroy`
+ Kiểm tra kỹ plan trước khi xác nhận thao tác destroy.

{{% notice warning %}}
NEED AN IMAGE + slide dọn dẹp thể hiện Terraform destroy xóa toàn bộ AWS stack và đưa account về trạng thái sạch.
{{% /notice %}}

{{< img "images/5-Workshop/5.5-Policy/s3-bucket-policy.png" "endpoint diagram" >}}

#### Lời kết
Cảm ơn bạn đã theo dõi bản trình bày. Dự án có thể được gỡ bỏ sạch sẽ bằng Terraform sau khi bạn hoàn thành demo hoặc kiểm thử.
