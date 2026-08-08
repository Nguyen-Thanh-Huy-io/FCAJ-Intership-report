---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---



# Bài thu hoạch “FCAJ Community Day 23/05/2026”

### Mục Tiêu Của Sự Kiện

- Xây dựng cầu nối và tiếp lửa đam mê cho sinh viên, những người đang đi làm cùng các chuyên gia trong ngành
- Phổ biến những kinh nghiệm thực chiến về nền tảng đám mây (cloud), thiết kế hệ thống và trí tuệ nhân tạo
- Tạo môi trường để giao lưu kết nối, cải thiện kỹ năng giao tiếp và xử lý các bài toán thực tế

### Danh Sách Diễn Giả

- **Gia Hưng (AWS Việt Nam)** - Đánh giá về bức tranh nhân sự IT hiện tại và nhấn mạnh giá trị của việc làm ra sản phẩm thật
- **Tịnh Trương** - Hướng dẫn cách truyền đạt ngữ cảnh (context) hiệu quả cho AI và cảnh báo về lỗi tư duy “Internet puller”
- **Hải Anh** - Trình bày về sức mạnh của Amazon Q và cách thức kết nối linh hoạt thông qua MCP
- **Thịnh Nguyễn** - Phân tích chiến lược giá Flat Rate Pricing của CloudFront đi kèm các phương án bảo mật tối ưu
- **Nhóm UTM** - Kể lại trải nghiệm 36 tiếng thi đấu hackathon để lập trình một ứng dụng AI chuyên tạo và sửa giao diện (UI)
- **Đức Đào** - Làm rõ bản chất khó đoán (tính bất định) của các mô hình ngôn ngữ lớn (LLM) dù cho đã set Temperature = 0
- **Vy Lâm** - Giới thiệu cấu trúc multi-agent ứng dụng vào hệ thống đánh giá điểm tín dụng cho startup quy mô doanh nghiệp

### Nội Dung Nổi Bật

#### Cơn sốt nhân lực Platform và DevOps

- Trí tuệ nhân tạo đang giúp việc lập trình trở nên ít tốn kém và nhanh chóng hơn bao giờ hết  
- Lượng phần mềm bùng nổ dẫn đến cơn khát kỹ sư có khả năng duy trì và vận hành hệ thống  
- Sinh viên nên hướng tới việc xây dựng các sản phẩm trọn vẹn, có tính ứng dụng cao thay vì chỉ làm các bản demo hời hợt  

#### Tránh trở thành một “Internet puller”

- Việc nhồi nhét vô tội vạ dữ liệu từ internet hay các plugin vào AI sẽ mang lại tác dụng ngược  
- Cần phải khoanh vùng nhiệm vụ và cung cấp ngữ cảnh rành mạch để AI hoạt động đúng hướng  

#### Tối ưu chi phí bằng CloudFront Flat Rate

- Gói cước Flat Rate là vị cứu tinh giúp doanh nghiệp không bị "sốc bill" khi lượng truy cập tăng đột biến hay bị tấn công DDoS  
- Việc kết hợp thêm VPC Origin và mTLS tạo ra một hàng rào bảo mật cực kỳ vững chắc  

#### Đặc tính bất định của LLM

- Kết quả trả về từ AI vẫn có thể sai khác dù đã khóa thông số Temperature ở mức 0  
- Điều này bắt nguồn từ những sai số khi làm tròn trong toán học và các tinh chỉnh từ phía server xử lý (inference)  

#### Sức mạnh của kiến trúc Multi-agent

- Là chìa khóa để phá vỡ giới hạn độ dài của context window trên LLM  
- Hỗ trợ việc phân chia quyền hạn rõ ràng, từ đó đáp ứng được các tiêu chuẩn bảo mật khắt khe của doanh nghiệp  

### Bài Học Rút Ra

#### Công nghệ sinh ra để phục vụ con người

- Mọi công cụ AI sẽ trở nên vô dụng nếu nó không giải quyết được bất kỳ nỗi đau nào của người dùng hoặc doanh nghiệp  
- "Sản phẩm này dành cho ai và để làm gì?" là câu hỏi bắt buộc phải trả lời trước khi bắt tay vào code  

#### Không bao giờ ngừng kiểm thử

- Do AI hoạt động dựa trên xác suất, hệ thống bắt buộc phải được thiết kế để dự phòng và xử lý các tình huống lỗi  
- Chỉ có quá trình testing liên tục mới đảm bảo được chất lượng hệ thống trước khi đến tay người dùng cuối  

#### Đừng nhắm mắt dùng code của AI

- Việc copy/paste trực tiếp mã nguồn do AI sinh ra vào các dự án lớn là một hành động cực kỳ rủi ro  
- Nếu không qua kiểm duyệt, những đoạn code này có thể phá vỡ cấu trúc và gây sập hệ thống  

#### Tốc độ là yếu tố sống còn

- Tiêu chuẩn và kỳ vọng của ngành công nghệ đang thay đổi chóng mặt qua từng tháng  
- Việc chậm trễ hành động sẽ khiến chúng ta phải trả giá rất đắt để đuổi kịp xu hướng  

### Trải Nghiệm Sự Kiện

Sự kiện đã thành công trong việc dung hòa giữa kiến thức học thuật chuyên sâu và các bài demo trực quan, đi kèm với sự tương tác rất nhiệt tình.

#### Gần gũi và đầy tính thực chiến
- Các diễn giả không ngần ngại kể lại những lần vấp ngã và thất bại khi triển khai dự án thực tế  
- Lối chia sẻ mộc mạc, đi thẳng vào vấn đề giúp người nghe dễ dàng tiếp thu kiến thức  

#### Khơi dậy sự tự tin
- Ban tổ chức liên tục khuấy động không khí bằng các câu hỏi tương tác và phần quà thú vị  
- Thông điệp xuyên suốt là hãy mạnh dạn thể hiện bản thân và xây dựng hình ảnh cá nhân (visibility) để tiến xa hơn trong sự nghiệp  

---
**Ảnh minh chứng sự kiện:**
{{< img "images/Workshop/Event2.png" "Minh chứng tham gia Event 2" >}}
