---
title: "Nhật ký Công việc Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Module 10** — Giám sát, tuân thủ và quản trị trên AWS

### Mục tiêu Tuần 10

- Phân biệt chỉ số vận hành, nhật ký ứng dụng và lịch sử thao tác API.
- Xác định bằng chứng tuân thủ của AWS và bằng chứng cần thu thập từ tài nguyên của người dùng.
- Giải thích cách quản trị nhiều tài khoản và xử lý các khuyến nghị vận hành.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Giám sát ứng dụng bằng Amazon CloudWatch**<ul><li>Phân biệt giám sát, kiểm toán, tuân thủ và quản trị. Dùng tình huống API Tindy trả nhiều lỗi 5xx để chọn metric, log group và khoảng thời gian cần xem.</li><li>Phác thảo dashboard cho số lượng target khỏe, tỷ lệ lỗi và CPU của ECS. Mô tả cách alarm đánh giá ngưỡng và gửi thông báo qua SNS khi cần người vận hành kiểm tra.</li></ul> | 16/11/2026 | 16/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Monitoring, Compliance, and Governance in the AWS Cloud<br>02 — Introduction to Monitoring<br>03 — Amazon CloudWatch |
| Thứ Ba | **Kiểm toán thao tác với AWS CloudTrail**<ul><li>Đọc một sự kiện mẫu để xác định ai thực hiện thao tác, API nào được gọi, lúc nào và tài nguyên nào liên quan. So sánh management events với data events.</li><li>Dùng tình huống security group thay đổi hoặc ECS được cập nhật qua CI/CD để phân biệt Event history với trail dùng lưu trữ phục vụ kiểm toán. Ghi cách đối chiếu thời điểm thay đổi với lỗi quan sát được trong CloudWatch.</li></ul> | 17/11/2026 | 17/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS CloudTrail |
| Thứ Tư | **Bằng chứng tuân thủ và cấu hình tài nguyên**<ul><li>Phân biệt báo cáo và thỏa thuận của AWS qua Artifact với yêu cầu tự kiểm tra cấu hình, chính sách và vị trí dữ liệu của ứng dụng.</li><li>Mô tả cách AWS Config ghi nhận cấu hình và đánh giá tài nguyên theo rule. Đọc ví dụ về framework, control, assessment và evidence của Audit Manager để hiểu cách thu thập bằng chứng được trình bày trong khóa học.</li></ul> | 18/11/2026 | 18/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Compliance<br>06 — Auditing AWS Resources for Compliance |
| Thứ Năm | **Quản trị nhiều tài khoản AWS**<ul><li>Vẽ cấu trúc AWS Organizations gồm management account, member account và OU. Phân biệt thanh toán hợp nhất với quản lý quyền.</li><li>Dùng ví dụ tách môi trường dev và production để giải thích SCP giới hạn phạm vi quyền có thể cấp. Liên hệ AWS Control Tower với landing zone, Account Factory và các control phục vụ quản trị nhiều tài khoản.</li></ul> | 19/11/2026 | 19/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — AWS Organizations<br>08 — Governance |
| Thứ Sáu | **AWS Health và AWS Trusted Advisor**<ul><li>Dùng ví dụ thông báo bảo trì Fargate để đọc phạm vi tài nguyên bị ảnh hưởng, thời gian và hành động đề xuất trong AWS Health.</li><li>So sánh sự kiện AWS Health với khuyến nghị Trusted Advisor. Chọn một kiểm tra về chi phí hoặc giới hạn dịch vụ, xác minh tài nguyên liên quan và ghi người chịu trách nhiệm xử lý.</li></ul> | 20/11/2026 | 20/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>09 — AWS Health<br>10 — AWS Trusted Advisor |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần 10 tập trung vào việc giám sát và quản trị hệ thống với Amazon CloudWatch và CloudTrail. Em nhận ra rằng một ứng dụng tốt không chỉ chạy được mà còn phải có khả năng quan sát (Observability) để phát hiện và xử lý sự cố kịp thời.

Trong quá trình kiểm thử giao diện Tindy, em đã kết hợp giữa việc kiểm tra console/network trên Chrome DevTools với việc theo dõi log thời gian thực trên CloudWatch. Khi thử nghiệm tính năng Rate Limiting, em có thể quan sát thấy request trả về mã 429 Too Many Requests trên trình duyệt đồng thời log cảnh báo được ghi lại tức thời trên CloudWatch Logs.

### Thành tựu Tuần 10

- CloudWatch giúp nhận biết tình trạng vận hành, còn CloudTrail cho phép lần lại thao tác API.
- AWS Artifact cung cấp tài liệu tuân thủ của AWS. AWS Config ghi nhận và đánh giá cấu hình tài nguyên theo quy tắc đã chọn.
- AWS Organizations và Control Tower hỗ trợ đặt quy tắc chung cho nhiều tài khoản. AWS Health và Trusted Advisor cung cấp đầu vào cho các công việc vận hành.
- **Áp dụng vào Tindy:** Kết hợp Chrome DevTools Network với CloudWatch Logs để giám sát mã phản hồi HTTP 101 WebSocket và phát hiện các request bị chặn do Rate Limit (429).


