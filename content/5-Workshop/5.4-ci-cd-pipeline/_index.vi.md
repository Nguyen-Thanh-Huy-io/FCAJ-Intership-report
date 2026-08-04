---
title : "Pipeline CI/CD"
date : 2024-01-01 
weight : 4 
chapter : false
pre : " <b> 5.4. </b> "
---

#### Module Terraform cho tự động hóa phát hành

Chương này giải thích cách repository tự động hóa luồng phát hành thông qua CodeStar, CodeBuild và CodePipeline.

#### Dịch vụ CI/CD do Terraform tạo ra
+ S3 bucket để lưu pipeline artifacts.
+ Kết nối CodeStar để lấy source từ GitHub.
+ IAM roles và policies cho CodePipeline và CodeBuild.
+ CodeBuild projects cho backend và frontend.
+ CodePipelines cho các giai đoạn phát hành backend và frontend.

#### Hành vi build
+ Backend build chạy ở chế độ privileged Docker vì cần build container image.
+ Frontend build xuất asset lên S3 bucket và invalidate CloudFront.
+ Cả hai pipeline đều lấy source từ cùng một GitHub branch được cấu hình trong Terraform.

{{% notice warning %}}
NEED AN IMAGE + sơ đồ CI/CD thể hiện GitHub, CodeStar connection, CodeBuild, CodePipeline, S3 artifacts, ECR, ECS và CloudFront.
{{% /notice %}}

{{< img "images/5-Workshop/5.4-S3-onprem/diagram3.png" "Interface endpoint architecture" >}}

#### Ý nghĩa
+ Việc phát hành được tái tạo và gắn với source control.
+ Logic build tách biệt khỏi source code ứng dụng.
+ Cùng một stack Terraform định nghĩa đường đi phát hành cho cả frontend và backend.



