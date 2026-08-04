---
title : "Kiến trúc và thiết lập"
date : 2024-01-01 
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

#### Các tài nguyên AWS do Terraform tạo ra

Chương này trình bày hạ tầng hỗ trợ ứng dụng và cách Terraform ghép các thành phần lại với nhau.

#### Dịch vụ AWS chính
+ VPC với public và private subnets để tách lớp mạng và workload.
+ ALB ở lớp public để nhận lưu lượng web.
+ ECS service và task definitions cho API và các worker nền.
+ RDS cho cơ sở dữ liệu quan hệ và ElastiCache Redis cho cache và queue.
+ ECR cho container images, S3 và CloudFront cho frontend, Route 53 cho domain, và Secrets Manager cho secret runtime.

#### Thuộc tính quan trọng
+ ECS service được đặt desired count là 1 API và 2 lớp worker.
+ Kết nối database sử dụng MySQL trên cổng 3306.
+ Terraform đưa environment variables và secret ARNs vào task definitions.
+ Frontend bucket được kết hợp với CloudFront để phân phối công khai.

{{% notice warning %}}
NEED AN IMAGE + sơ đồ tổng thể thể hiện VPC, ALB, ECS, RDS, Redis, ECR, S3/CloudFront, Route 53 và Secrets Manager.
{{% /notice %}}

{{< img "images/5-Workshop/5.3-S3-vpc/diagram2.png" "overview" >}}

#### Nội dung

- [Bố cục hạ tầng](5.3.1-infrastructure-layout/)
- [Thuộc tính tài nguyên](5.3.2-resource-properties/)