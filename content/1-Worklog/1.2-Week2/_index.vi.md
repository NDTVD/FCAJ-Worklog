---
title: "Nhật ký Công việc Tuần 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Module 2** — Dịch vụ Compute (EC2), Cân bằng Tải (ELB) và Nhắn tin Hàng đợi

### Mục tiêu Tuần 2

- Lựa chọn các họ máy chủ ảo Amazon EC2 (General Purpose, Compute/Memory/Storage Optimized) phù hợp với từng loại workload.
- Hiểu cơ chế hoạt động của Elastic Load Balancing (ALB), Auto Scaling Groups và cách thực hiện kiểm tra sức khỏe (Health Check).
- Nắm bắt nguyên lý tách rời hệ thống (Decoupling) bằng dịch vụ hàng đợi thông điệp Amazon SQS và thông báo đẩy Amazon SNS.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Khảo sát Họ máy chủ EC2 & Vòng đời Instance**<ul><li>Tìm hiểu nguyên lý ảo hóa máy chủ. Phân loại các họ instance: dòng T/M cho mục đích đa dụng, dòng C cho tác vụ CPU cao, dòng R cho bộ nhớ lớn, và dòng I/D cho lưu trữ tốc độ cao.</li><li>Phân tích vòng đời của EC2: Pending, Running, Stopping, Stopped và Terminated. Ghi nhận sự khác biệt về chi phí lưu trữ và địa chỉ IP khi tạm dừng instance so với hủy hoàn toàn.</li></ul> | 21/09/2026 | 21/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Amazon EC2<br>02 — Amazon EC2 Instance Types |
| Thứ Ba | **Cấu hình Khởi tạo Máy chủ Web EC2 Thực tế**<ul><li>Nghiên cứu quy trình khởi tạo máy chủ qua Console, AWS CLI và SDK. Tìm hiểu vai trò của Amazon Machine Image (AMI), Key Pair để đăng nhập SSH, và Security Group điều khiển cổng mạng (Port 80/443).</li><li>Phân tích đoạn mã User Data script: cách tự động cập nhật hệ điều hành, cài đặt web server Nginx/Apache và clone mã nguồn ứng dụng ngay trong lần đầu instance khởi động.</li></ul> | 22/09/2026 | 22/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — How to Provision AWS Resources<br>04 — Demo Launching an Amazon EC2 Instance |
| Thứ Tư | **Các Mô hình Định giá Amazon EC2**<ul><li>So sánh 5 mô hình mua EC2: On-Demand (trả theo giây, linh hoạt cao nhất), Savings Plans / Reserved Instances (cam kết 1-3 năm để giảm đến 72% chi phí), Spot Instances (tận dụng năng lực dư thừa với giá rẻ đến 90% cho tác vụ có thể chịu gián đoạn), và Dedicated Hosts.</li><li>Xây dựng ma trận lựa chọn mô hình mua phù hợp cho môi trường phát triển (Dev/Test) so với môi trường vận hành chính thức (Production).</li></ul> | 23/09/2026 | 23/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon EC2 Pricing |
| Thứ Năm | **Tự động Mở rộng (Auto Scaling) & Cân bằng Tải (ALB)**<ul><li>Phân biệt mở rộng theo chiều dọc (Scale Up) và mở rộng theo chiều ngang (Scale Out). Tìm hiểu cách Auto Scaling Group tự động thêm/bớt instance dựa trên ngưỡng CPUUtilization từ CloudWatch.</li><li>Nghiên cứu cơ chế điều phối của Application Load Balancer: định tuyến theo đường dẫn (Path-based routing), chuyển tiếp kết nối WebSocket và sử dụng Health Checks (`/healthz` trả về HTTP 200) để cô lập instance gặp lỗi.</li></ul> | 24/09/2026 | 24/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Scaling Amazon EC2<br>07 — Directing Traffic with Elastic Load Balancing |
| Thứ Sáu | **Kiến trúc Bất đồng bộ với Amazon SQS và Amazon SNS**<ul><li>Khảo sát mô hình Publish/Subscribe của SNS và hàng đợi Message Queue của SQS. Phân tích mô hình Fanout: một sự kiện được SNS phát tán đồng thời tới nhiều hàng đợi SQS độc lập.</li><li>So sánh hàng đợi Standard Queue (thông lượng cực cao, đảm bảo giao ít nhất một lần nhưng có thể lệch thứ tự) và FIFO Queue (đảm bảo thứ tự nghiêm ngặt và không trùng lặp). Đặt vào tình huống xử lý tệp upload của người dùng.</li></ul> | 25/09/2026 | 25/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Messaging and Queuing |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Trong tuần học về Compute và Messaging, em đặc biệt chú ý đến cách thức Elastic Load Balancing (ALB) điều phối lưu lượng truy cập. Với vai trò Frontend phụ trách tính năng Chat thời gian thực trên Tindy, em nhận thấy ALB không chỉ đơn thuần phân chia HTTP request mà còn phải hỗ trợ duy trì kết nối WebSocket liên tục để người dùng không bị rớt kết nối SignalR khi đang nhắn tin.

Bên cạnh đó, việc tìm hiểu về Amazon SQS và SNS mang lại cho em tư duy thiết kế bất đồng bộ (asynchronous decoupling). Thay vì bắt người dùng phải chờ đợi trình duyệt xoay vòng khi upload tệp CV PDF nặng, hệ thống có thể tiếp nhận yêu cầu ngay lập tức và đẩy tác vụ quét virus, trích xuất AI vào hàng đợi ngầm phía sau, giúp tối ưu hóa đáng kể trải nghiệm tương tác (UX) của người dùng.

### Thành tựu Tuần 2

- Lựa chọn đúng họ instance EC2 và mô hình giá phù hợp giúp tiết kiệm đáng kể ngân sách mà vẫn đảm bảo hiệu năng xử lý.
- Application Load Balancer kết hợp Auto Scaling Group mang lại khả năng chịu lỗi và tự phục hồi khi có máy chủ gặp sự cố.
- Áp dụng vào Tindy: Hiểu cách Application Load Balancer (ALB) điều phối lưu lượng và duy trì kết nối WebSocket liên tục cho khung chat SignalR hai chiều.
