---
title: "Nhật ký Công việc Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Module 9** — Bảo mật, Quản lý Định danh (IAM) và Gia cố Ứng dụng Web

### Mục tiêu Tuần 9

- Áp dụng nguyên tắc đặc quyền tối thiểu (Least Privilege) với AWS Identity and Access Management (IAM): Users, Roles và Policies.
- Hiểu rõ các tầng bảo vệ ứng dụng đám mây: mã hóa dữ liệu với AWS KMS, quản lý bí mật AWS Secrets Manager và tường lửa AWS WAF.
- Trực tiếp triển khai các giải pháp bảo mật ứng dụng web: chính sách CORS chặt chẽ và cơ chế Rate Limiting chống spam tin nhắn.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Quản lý Định danh AWS IAM & Nguyên tắc Đặc quyền Tối thiểu**<ul><li>Khảo sát các thành phần IAM: IAM User (người dùng cá nhân), IAM Group (nhóm người dùng), IAM Policy (văn bản cấp quyền định dạng JSON) và IAM Role (vai trò ủy quyền tạm thời).</li><li>Phân tích nguyên tắc Least Privilege: chỉ cấp đúng những quyền tối thiểu cần thiết để hoàn thành công việc; cấm sử dụng tài khoản Root cho các hoạt động phát triển hằng ngày.</li></ul> | 09/11/2026 | 09/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Security on AWS<br>02 — Preventing Unauthorized Access |
| Thứ Ba | **IAM Roles cho Dịch vụ AWS & Xác thực OIDC GitHub Actions**<ul><li>Tìm hiểu cách gán IAM Role cho máy chủ EC2 hoặc ECS Task: tự động cung cấp thông tin xác thực tạm thời thông qua AWS Security Token Service (STS) mà không cần lưu khóa truy cập bí mật trên máy chủ.</li><li>Nghiên cứu cơ chế OpenID Connect (OIDC) giữa GitHub Actions và AWS: cho phép pipeline CI/CD triển khai code lên S3 và CloudFront một cách an toàn mà không cần lưu AWS Access Key tĩnh trong kho lưu trữ Git.</li></ul> | 10/11/2026 | 10/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Protecting Networks and Applications |
| Thứ Tư | **Mã hóa Dữ liệu AWS KMS & Quản lý Bí mật Secrets Manager**<ul><li>Khảo sát dịch vụ quản lý khóa mã hóa AWS Key Management Service (KMS): mã hóa dữ liệu khi lưu trữ (Encryption at Rest) trên S3, EBS và RDS.</li><li>Tìm hiểu AWS Secrets Manager: lưu trữ chuỗi kết nối cơ sở dữ liệu PostgreSQL, mã bí mật JWT và tự động xoay vòng khóa (Automatic Secret Rotation) định kỳ.</li></ul> | 11/11/2026 | 11/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Protecting Data |
| Thứ Năm | **Tường lửa Ứng dụng AWS WAF & Cấu hình CORS trong Mã nguồn**<ul><li>Nghiên cứu AWS WAF (Web Application Firewall): ngăn chặn các cuộc tấn công web phổ biến như SQL Injection, Cross-Site Scripting (XSS) và giới hạn tần suất yêu cầu HTTP (Rate-based rules) tại tầng CloudFront/ALB.</li><li>Trực tiếp triển khai cấu hình chính sách CORS trong file `Program.cs` của backend: chỉ cho phép các request đến từ tên miền CloudFront chính thức của Tindy, mở các phương thức GET, POST, PUT, DELETE, OPTIONS.</li></ul> | 12/11/2026 | 12/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Detecting and Responding to Security Incidents |
| Thứ Sáu | **Triển khai Cơ chế Giới hạn Tần suất Tin nhắn (Rate Limiting)**<ul><li>Phân tích rủi ro khi tính năng Chat thời gian thực bị kẻ xấu spam tin nhắn liên tục: làm nghẽn hàng đợi WebSocket, tràn bộ nhớ RAM của server và quấy rầy trải nghiệm người dùng.</li><li>Xây dựng logic điều tiết tần suất (Message Throttling / Rate Limiting): giới hạn mỗi người dùng chỉ được gửi tối đa một số lượng tin nhắn nhất định trong một cửa sổ thời gian (ví dụ: tối đa 5 tin/giây); trả về cảnh báo khi vượt ngưỡng.</li></ul> | 13/11/2026 | 13/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Additional Security Resources |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần học về Security là tuần em có đóng góp kỹ thuật trực tiếp nhất vào mã nguồn của dự án Tindy. Trong quá trình phát triển tính năng Chat thời gian thực giữa các thành viên dự án, em nhận thấy nguy cơ người dùng bấm gửi liên tục hoặc dùng script để spam khung chat, làm tràn bộ nhớ trình duyệt của người nhận và nghẽn máy chủ.

Em đã nghiên cứu và triển khai cơ chế Giới hạn tốc độ gửi tin nhắn (Message Rate Limiting / Throttling). Khi người dùng gửi tin quá nhanh, hệ thống sẽ tạm thời chặn và hiển thị thông báo nhắc nhở nhẹ nhàng trên giao diện. Đồng thời, việc cấu hình CORS chặt chẽ trong `Program.cs` giúp đảm bảo chỉ có trang web chính thức của nhóm mới có thể giao tiếp với API backend, loại bỏ hoàn toàn các request giả mạo từ bên ngoài.

### Thành tựu Tuần 9

- Nguyên tắc đặc quyền tối thiểu (Least Privilege) và việc sử dụng IAM Role thay cho Access Key tĩnh là quy chuẩn bảo mật bắt buộc trên đám mây.
- Bảo mật ứng dụng web đòi hỏi sự kết hợp giữa tường lửa hạ tầng (WAF), cấu hình mạng (CORS) và logic nghiệp vụ ứng dụng (Rate Limiting).
- Áp dụng vào Tindy: Cấu hình chính sách CORS trong Program.cs của backend; xây dựng tính năng giới hạn tần suất gửi tin nhắn (Rate Limiting) trong dịch vụ chat để chống spam.
