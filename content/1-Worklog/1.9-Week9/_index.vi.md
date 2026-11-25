---
title: "Nhật ký Công việc Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Module 9** — Bảo mật, bảo vệ dữ liệu và xử lý phát hiện

### Mục tiêu Tuần 9

- Phân biệt xác thực, phân quyền và trách nhiệm của AWS với trách nhiệm của người dùng.
- Chọn biện pháp bảo vệ ở lớp mạng, ứng dụng và dữ liệu.
- Xác định vai trò của từng dịch vụ trong luồng phát hiện và điều tra sự cố.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Danh tính và quyền truy cập**<ul><li>Phân biệt xác thực và phân quyền bằng ví dụ người dùng đăng nhập Tindy rồi truy cập một tài nguyên. Ôn cách bảo vệ tài khoản root bằng MFA và dùng danh tính phù hợp cho công việc hằng ngày.</li><li>Đọc IAM policy theo principal, hành động và tài nguyên. Dùng task role của ECS truy cập S3 làm tình huống áp dụng quyền tối thiểu, rồi so sánh với quyền của người dùng qua IAM Identity Center.</li></ul> | 09/11/2026 | 09/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Security on AWS<br>02 — Preventing Unauthorized Access |
| Thứ Ba | **Bảo vệ mạng và ứng dụng**<ul><li>Lần theo chuỗi CloudFront, ALB và ECS để xác định luồng lưu lượng nào cần được cho phép ở mỗi security group.</li><li>So sánh vai trò của AWS WAF khi lọc yêu cầu ở lớp ứng dụng với vai trò của AWS Shield trong bảo vệ trước DDoS. Ghi rõ thành phần nào thuộc ví dụ bảo mật nhiều lớp của khóa học khi liên hệ kiến trúc Tindy.</li></ul> | 10/11/2026 | 10/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Protecting Networks and Applications |
| Thứ Tư | **Mã hóa và bảo vệ dữ liệu**<ul><li>Phân biệt mã hóa khi lưu trữ trong S3 hoặc EBS với mã hóa khi truyền qua TLS. Dùng một tài liệu tải lên để xác định các điểm dữ liệu đi qua.</li><li>Đối chiếu vai trò quản lý khóa của AWS KMS với vai trò quản lý chứng chỉ của ACM. Ghi các quyền cần rà soát khi dịch vụ truy cập dữ liệu đã mã hóa, gồm quyền trên tài nguyên và quyền dùng khóa khi áp dụng.</li></ul> | 11/11/2026 | 11/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Protecting Data |
| Thứ Năm | **Phát hiện và điều tra sự cố**<ul><li>Lập bảng vai trò: Inspector phát hiện lỗ hổng, GuardDuty tạo phát hiện về mối đe dọa, Detective hỗ trợ điều tra và Security Hub tập hợp thông tin bảo mật.</li><li>Dùng một cảnh báo mẫu để xác định tài nguyên, thời điểm và nguồn bằng chứng cần kiểm tra. Liên hệ việc ghi nhận cảnh báo với bước xác minh ảnh hưởng trước khi chọn cách xử lý.</li></ul> | 12/11/2026 | 12/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Detecting and Responding to Security Incidents |
| Thứ Sáu | **Tra cứu và đánh giá nguồn bảo mật**<ul><li>Xác định khi nào cần xem tài liệu AWS để hiểu cấu hình, Knowledge Center để tra lỗi và AWS Security Blog để tìm bối cảnh của một cách triển khai.</li><li>Đọc một tình huống chọn giải pháp bảo mật từ AWS Marketplace. Lập tiêu chí đánh giá phạm vi quyền, chi phí, trách nhiệm vận hành và mức độ phù hợp với hạ tầng trước khi quyết định dùng.</li></ul> | 13/11/2026 | 13/11/2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Additional Security Resources |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Module 9 trang bị cho em kiến thức toàn diện về bảo mật đám mây: từ nguyên tắc đặc quyền tối thiểu (Least Privilege) của AWS IAM đến các lớp tường lửa Security Group và AWS WAF.

Ở cấp độ ứng dụng, em đã trực tiếp vận dụng các bài học bảo mật để tối ưu hóa hai thành phần Backend của Tindy:
1. Kiểm soát CORS: Chỉ cho phép đúng domain CloudFront và localhost gửi request kèm cookie/header xác thực, ngăn chặn nguy cơ tấn công Cross-Origin.
2. Cơ chế Message Rate Limiting: Thiết lập middleware giới hạn tần suất gửi tin nhắn trong khung chat SignalR, ngăn chặn hành vi spam hoặc flood request gây cạn kiệt tài nguyên container Fargate.

### Thành tựu Tuần 9

- IAM và quyền tối thiểu giới hạn những gì từng danh tính hoặc workload được làm.
- Security group, WAF, Shield, TLS và mã hóa khi lưu trữ phục vụ các lớp bảo vệ khác nhau.
- Một phát hiện bảo mật là đầu vào cho quá trình xác minh tài nguyên, dấu thời gian và ảnh hưởng.
- **Áp dụng vào Tindy:** Trực tiếp cấu hình chính sách CORS trong ASP.NET Core để FE gọi API qua CloudFront an toàn, đồng thời triển khai Message Rate Limiting chống spam chat.


