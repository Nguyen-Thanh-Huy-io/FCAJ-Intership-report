---
title: "Tự đánh giá & Nhìn lại chặng đường"
weight: 7
---

> Nhìn lại hành trình xây dựng và triển khai dự án PubliCast từ một nguyên mẫu (prototype) cục bộ lên một kiến trúc AWS chuẩn production, dưới đây là những suy ngẫm cá nhân, những thách thức đã vượt qua và các bài học cốt lõi tôi nhận được từ chương trình First Cloud AI Journey (FCAJ).

### Đánh giá Tổng quan

**1. Sự trưởng thành về Kỹ thuật & Làm chủ Đám mây**  
Trước dự án này, hiểu biết của tôi về hạ tầng đám mây chủ yếu nằm ở lý thuyết. Thông qua chương trình FCAJ, tôi đã chuyển sang cách tiếp cận thực hành sâu. Việc tự tay thiết kế VPC, thiết lập các container ECS Fargate và cấu hình Application Load Balancer đã mang lại cho tôi cái nhìn thực tế và sâu sắc về cách các hệ thống quy mô lớn vận hành.

**2. Sức mạnh của Infrastructure as Code (IaC)**  
Một trong những khía cạnh thỏa mãn nhất là học và sử dụng Terraform. Thay vì phải thao tác thủ công trên giao diện AWS Console, việc có thể định nghĩa toàn bộ hạ tầng bằng code, tự động triển khai hoặc phá hủy chúng một cách trơn tru thực sự là một bước ngoặt lớn. Nó dạy tôi tầm quan trọng của tính tự động hóa và khả năng tái sử dụng trong DevOps.

**3. Tư duy Thiết kế Kiến trúc**  
Quá trình làm dự án buộc tôi phải suy nghĩ nghiêm túc về những sự đánh đổi (trade-offs) trong kiến trúc. Ví dụ: việc tách rời backend nguyên khối thành dịch vụ API và các worker chạy ngầm (Worker Light/Heavy) khá phức tạp nhưng cực kỳ cần thiết. Nó làm nổi bật bài học về việc ưu tiên độ bền bỉ của hệ thống và trải nghiệm người dùng hơn là tốc độ code nhanh.

**4. Sự hỗ trợ từ Mentor & Cộng đồng**  
Sự hỗ trợ từ các mentor FCAJ và cộng đồng là vô giá. Bất cứ khi nào tôi gặp phải các vấn đề phức tạp — như gỡ lỗi VPC S3 Endpoints hay cấu hình CloudFront OAC — sự hướng dẫn tôi nhận được luôn kịp thời và mang tính khích lệ cao. Điều này củng cố thêm tầm quan trọng của việc hợp tác giải quyết vấn đề trong ngành công nghệ thông tin.

---

### Những Thách thức Đã vượt qua
- **Độ phức tạp của Networking:** Việc hiểu cách tương tác giữa Public/Private Subnets, NAT Gateways và Security Groups ban đầu khá choáng ngợp. Nhưng nhờ việc vẽ sơ đồ và trực tiếp kiểm thử, các khái niệm đã trở nên rõ ràng và logic hơn.
- **Điều phối CI/CD:** Thiết lập AWS CodePipeline cho một monorepo đòi hỏi khả năng lọc đường dẫn (path filtering) chính xác và phân quyền IAM nghiêm ngặt. Đây là một bài học bảo mật khó nhằn nhưng cực kỳ đáng giá.

---

### Định hướng Tương lai
- **Bước tiếp theo cho PubliCast:** Tôi dự định mở rộng nền tảng bằng cách tích hợp các luồng tạo nội dung tự động bằng AI và mở rộng trang tổng quan phân tích dữ liệu (analytics dashboard).
- **Mục tiêu Cá nhân:** Tiếp tục đào sâu vào các công nghệ AWS Serverless (như Lambda, EventBridge) và chinh phục các chứng chỉ AWS chuyên nghiệp.

*Xin gửi lời cảm ơn chân thành tới đội ngũ FCAJ vì cơ hội học tập tuyệt vời này!*