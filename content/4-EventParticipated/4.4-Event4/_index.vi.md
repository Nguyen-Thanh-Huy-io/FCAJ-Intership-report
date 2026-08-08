---
title: "Event 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---



# Bài thu hoạch “FCAJ Community Day 27/06/2026”

### Mục Tiêu Của Sự Kiện

- Trình làng những giải pháp Trí tuệ nhân tạo (AI) có tính ứng dụng cao dành cho khối doanh nghiệp
- Trực quan hóa cách các công cụ AI của hệ sinh thái AWS tháo gỡ các nút thắt trong khâu chăm sóc khách hàng, vận hành DevOps và quản trị nhân sự (HR)
- Đề cao tầm quan trọng của việc triển khai AI một cách an toàn và khả năng tương thích với hạ tầng mạng có sẵn

### Danh Sách Diễn Giả

- **Anh Kiệt & Anh Trung (RAI)** - Giới thiệu các ứng dụng Voice Agent và bài toán hóc búa khi xây dựng tổng đài bằng tiếng Việt
- **Nguyên & Chị Bảo** - Hướng dẫn cách dùng AWS DevOps AI Agent để tự động truy vết và khắc phục lỗi hệ thống
- **Trường (Wayne) & Minh Anh (Noventiq)** - Giới thiệu giải pháp Amazon Q Business chuyên biệt hóa cho mảng tuyển dụng và sàng lọc ứng viên
- **Toàn Nguyễn (Security Builder) & Anh Nghị (Ra Club)** - Đào sâu vào các thiết kế mạng bảo mật nội bộ khi cần kết nối Amazon Q với các máy chủ MCP riêng của công ty

### Nội Dung Nổi Bật

#### Voice AI thuần Việt

- Do tiếng Việt thuộc nhóm ngôn ngữ thiếu hụt dữ liệu huấn luyện (low-resource), hệ thống đòi hỏi một cơ chế xử lý âm thanh cực kỳ tinh tế  
- Kiến trúc tổng thể là sự kết hợp nhịp nhàng giữa STT (chuyển giọng nói thành văn bản), LLM (để phân tích ngữ cảnh) và TTS (chuyển văn bản thành giọng nói)  
- Mô hình được "dạy" cách xử lý các tình huống bị ngắt lời, dùng đúng đại từ nhân xưng và nhận diện chính xác các âm sắc vùng miền  

#### Giải phóng sức lao động DevOps nhờ AI Agent

- Trợ lý AWS DevOps AI Agent tự động gom nhặt và phân tích các bản log/trace để truy tìm tận gốc rễ nguyên nhân gây lỗi  
- Công cụ này có thể biến một quy trình điều tra kéo dài hàng tuần lễ xuống chỉ còn vài phút ngắn ngủi  
- Nhiều tổ chức lớn như WGU hay KDI đã áp dụng thành công mô hình này để tối ưu hóa thời gian xử lý sự cố (incident response)  

#### Amazon Q - Trợ thủ đắc lực cho HR

- Các chuyên viên nhân sự thường bị quá tải bởi việc phải đọc và phân loại CV bằng mắt thường  
- Với Amazon Q, hệ thống sẽ tự động quét CV, bóc tách các kỹ năng cốt lõi, so sánh đối chiếu với yêu cầu công việc (JD) và đưa ra điểm số đánh giá ứng viên  

#### Thiết lập rào chắn bảo mật cho Amazon Q

- Việc luân chuyển dữ liệu được giữ kín hoàn toàn trong mạng nội bộ thông qua sự kết hợp của AWS VPC, ALB và Route 53 Resolver  
- Cách tiếp cận này tuân thủ nghiêm ngặt triết lý bảo mật Zero Trust, triệt tiêu hoàn toàn rủi ro lộ lọt dữ liệu nhạy cảm ra môi trường internet công cộng  

### Bài Học Rút Ra

#### AI là đòn bẩy, không phải kẻ thay thế

- AI Agent rất giỏi trong việc tóm tắt thông tin, đưa ra đề xuất và chấm điểm sơ bộ  
- Tuy nhiên, quyền quyết định tối hậu và những đánh giá mang tính chiến lược vẫn luôn thuộc về con người  

#### Dữ liệu là vua

- AI chỉ có thể "thông minh" khi được nuôi dưỡng bằng một hệ thống dữ liệu đồ sộ gồm log, cảnh báo (alert) và lịch sử hoạt động  
- Một hệ thống hạ tầng càng quy củ và trưởng thành thì kết quả do AI trả về mới thực sự có giá trị  

#### Chìa khóa nằm ở tính tương thích

- Doanh nghiệp không cần phải tự trói mình vào một nhà cung cấp dịch vụ duy nhất  
- Thông qua giao thức MCP, Amazon Q hoàn toàn có thể bắt tay mượt mà với các nền tảng khác như SharePoint, Google Workspace, Jira hay các máy chủ tự vận hành (self-hosted)  

### Trải Nghiệm Sự Kiện

Chương trình mang đậm tính kỹ thuật ứng dụng, dành phần lớn thời lượng cho việc chạy demo các dự án thực tế.

#### Mắt thấy tai nghe
- Khán giả được chứng kiến các diễn giả thao tác trực tiếp trên các hệ thống có quy mô tương đương môi trường thật (production-like)  
- Cảm giác rất chân thực khi quan sát cách AI tự động chặn đứng một cuộc tấn công DDoS giả lập hay tự động chấm điểm một bộ hồ sơ xin việc  

#### Không khí thảo luận sôi nổi
- Ban tổ chức rất khéo léo lồng ghép các mini-game có thưởng để giữ nhịp độ chương trình luôn hào hứng  
- Người tham dự liên tục đặt ra những câu hỏi hóc búa, đi sâu vào cấu trúc kỹ thuật, chính sách giá và các tình huống vận hành hệ thống thực tế  

---
**Ảnh minh chứng sự kiện:**
{{< img "images/Workshop/Event4.png" "Minh chứng tham gia Event 4" >}}
