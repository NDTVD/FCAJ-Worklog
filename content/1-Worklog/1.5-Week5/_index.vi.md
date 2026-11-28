---
title: "Nhật ký Công việc Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Module 5** — Mạng Đám mây (Amazon VPC), Định tuyến và Kết nối API

### Mục tiêu Tuần 5

- Thiết kế cấu trúc mạng ảo biệt lập Amazon VPC với dải mạng CIDR, phân chia Public Subnets và Private Subnets an toàn.
- Phân biệt cơ chế hoạt động của Internet Gateway, NAT Gateway và bảng định tuyến Route Tables trong việc điều phối luồng dữ liệu.
- Làm chủ cơ chế bảo mật mạng đa lớp với Security Groups, Network ACLs và cấu hình chính sách Cross-Origin Resource Sharing (CORS) cho ứng dụng web.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Thiết kế Amazon VPC & Phân chia Dải mạng Subnets**<ul><li>Khảo sát nguyên lý mạng ảo cô lập Amazon VPC và cách chia dải địa chỉ IP theo ký hiệu CIDR block (ví dụ /16 và /24).</li><li>Phân tích mô hình mạng đa tầng: đặt Application Load Balancer ở Public Subnet có gắn Internet Gateway, đưa ECS Fargate backend và RDS Database vào Private Subnet không có IP công khai để bảo vệ dữ liệu.</li></ul> | 12/10/2026 | 12/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Networking<br>02 — Organizing AWS Cloud Resources |
| Thứ Ba | **Cổng Mạng Internet Gateway, NAT Gateway & Route Tables**<ul><li>Nghiên cứu vai trò của Internet Gateway trong việc cho phép lưu lượng truy cập hai chiều giữa Public Subnet và mạng Internet toàn cầu.</li><li>Tìm hiểu NAT Gateway đặt tại Public Subnet: cho phép các container trong Private Subnet gọi ra Internet (tải thư viện NuGet, gọi API Bedrock) nhưng chặn hoàn toàn các kết nối chủ động từ bên ngoài vào.</li></ul> | 13/10/2026 | 13/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — More Ways to Connect to the AWS Cloud |
| Thứ Tư | **Bảo mật Tầng Mạng: Security Groups vs Network ACLs**<ul><li>So sánh Security Group (tường lửa kiểm soát trạng thái - Stateful, hoạt động ở cấp độ instance/task) và Network ACL (tường lửa không kiểm soát trạng thái - Stateless, hoạt động ở cấp độ subnet).</li><li>Thiết lập quy tắc tường lửa nghiêm ngặt: Security Group của ECS chỉ chấp nhận traffic từ Security Group của ALB trên cổng HTTP; Security Group của Database chỉ chấp nhận kết nối cổng 5432 từ ECS.</li></ul> | 14/10/2026 | 14/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Subnets, Security Groups, and Network Access Control Lists<br>05 — Amazon VPC Demo |
| Thứ Năm | **Cấu hình CORS & Giải quyết Vấn đề Giao tiếp Tên miền**<ul><li>Phân tích cơ chế Cross-Origin Resource Sharing (CORS) khi trình duyệt web gửi HTTP request từ domain CloudFront (`*.cloudfront.net`) tới API backend (`*.elb.amazonaws.com`).</li><li>Tìm hiểu quy trình gửi preflight request `OPTIONS` của trình duyệt và cấu hình các headers bắt buộc: `Access-Control-Allow-Origin`, `Access-Control-Allow-Headers`, `Access-Control-Allow-Methods` để tránh lỗi chặn kết nối giao diện.</li></ul> | 15/10/2026 | 15/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Global Networking |
| Thứ Sáu | **Kiểm thử Kết nối Mạng Đầu Cuối & Đo lường Độ trễ**<ul><li>Thực hành kiểm tra định tuyến mạng thông qua công cụ cURL và browser developer network tab; xác minh response header và trạng thái kết nối HTTP 200.</li><li>Đánh giá luồng dữ liệu trọn vẹn: từ máy khách người dùng qua CloudFront Edge, định tuyến tới ALB ở Public Subnet, chuyển tiếp tới ECS trong Private Subnet và truy vấn RDS an toàn.</li></ul> | 16/10/2026 | 16/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Global Architectures |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Là lập trình viên Frontend, vấn đề em thường gặp nhất khi kết nối giao diện React với máy chủ chính là lỗi CORS (Cross-Origin Resource Sharing). Tuần học về VPC và Network này đã giúp em hiểu rõ bản chất tại sao trình duyệt lại chặn các request từ domain giao diện đến domain API khác nguồn.

Hiểu được cơ chế Preflight OPTIONS request và cách cấu hình các header CORS từ tầng mạng và backend giúp em chủ động phối hợp cùng nhóm giải quyết triệt để vấn đề này trên Tindy. Ngoài ra, việc thiết kế mô hình Private Subnet cho database và container backend giúp em an tâm tuyệt đối về tính bảo mật của toàn bộ hệ thống.

### Thành tựu Tuần 5

- Phân chia Public và Private Subnet kết hợp NAT Gateway là tiêu chuẩn hàng đầu để bảo vệ dữ liệu và dịch vụ nội bộ.
- Security Group hoạt động theo cơ chế Stateful giúp kiểm soát chính xác lưu lượng giữa các thành phần ứng dụng theo nguyên tắc đặc quyền tối thiểu.
- Áp dụng vào Tindy: Nghiên cứu luồng mạng giữa CloudFront, ALB và ECS; phối hợp cấu hình chính sách CORS trên backend để giao diện React kết nối thông suốt.
