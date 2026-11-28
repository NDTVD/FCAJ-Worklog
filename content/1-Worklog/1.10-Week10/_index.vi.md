---
title: "Nhật ký Công việc Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Module 10** — Giám sát Hệ thống (CloudWatch), Nhật ký Kiểm toán (CloudTrail) và Khắc phục Sự cố

### Mục tiêu Tuần 10

- Làm chủ hệ thống giám sát Amazon CloudWatch: thu thập số liệu (Metrics), gom nhật ký tập trung (Logs) và tạo bảng điều khiển trực quan (Dashboards).
- Thiết lập các cảnh báo tự động (CloudWatch Alarms) kích hoạt thông báo qua Amazon SNS khi phát hiện sự cố hệ thống.
- Kết hợp nhật ký kiểm toán AWS CloudTrail với kỹ thuật giám sát lỗi phía trình duyệt (Client-side Observability) để chẩn đoán sự cố nhanh chóng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Thu thập Chỉ số Hệ thống với Amazon CloudWatch Metrics**<ul><li>Khảo sát các chỉ số hiệu năng chuẩn: CPUUtilization và MemoryUtilization của ECS Tasks, số lượng request và HTTP 5XX error rate trên Application Load Balancer, và số kết nối Database.</li><li>Xây dựng CloudWatch Dashboard: tạo các biểu đồ trực quan hóa dữ liệu theo thời gian thực giúp đội ngũ kỹ thuật theo dõi sức khỏe tổng thể của ứng dụng chỉ trên một màn hình duy nhất.</li></ul> | 16/11/2026 | 16/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Monitoring, Compliance, and Governance in the AWS Cloud<br>02 — Introduction to Monitoring<br>03 — Amazon CloudWatch |
| Thứ Ba | **Gom Nhật ký Tập trung với Amazon CloudWatch Logs**<ul><li>Tìm hiểu cơ chế gom log của các container chạy trên ECS Fargate thông qua log driver `awslogs`: đẩy toàn bộ log stdout/stderr vào CloudWatch Log Groups.</li><li>Thực hành sử dụng công cụ CloudWatch Logs Insights: viết các câu truy vấn lọc lỗi `ERROR` hoặc `Exception` trong mã nguồn ASP.NET Core để tìm ra nguyên nhân gây lỗi sập endpoint API.</li></ul> | 17/11/2026 | 17/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS CloudTrail |
| Thứ Tư | **Thiết lập Cảnh báo Tự động (CloudWatch Alarms) & Thông báo SNS**<ul><li>Cấu hình các chỉ số cảnh báo: cảnh báo khi tỷ lệ phản hồi lỗi HTTP 5XX vượt quá 5% trong 5 phút, cảnh báo khi dung lượng RAM của container chạm ngưỡng 85%.</li><li>Thiết lập hành động khi Alarm chuyển sang trạng thái `ALARM`: kích hoạt Amazon SNS gửi email cảnh báo tức thì tới nhóm vận hành và tự động thêm bản sao container.</li></ul> | 18/11/2026 | 18/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Compliance<br>06 — Auditing AWS Resources for Compliance |
| Thứ Năm | **Theo dõi Nhật ký Kiểm toán với AWS CloudTrail**<ul><li>Khảo sát AWS CloudTrail: dịch vụ ghi lại toàn bộ lịch sử hoạt động và các lệnh gọi API trên tài khoản AWS.</li><li>Phân tích cấu trúc sự kiện CloudTrail: ai (Identity) đã tạo hoặc xóa tài nguyên nào, vào thời điểm nào (Timestamp), từ địa chỉ IP nào và thông qua Console hay CLI; phục vụ mục đích kiểm toán an ninh.</li></ul> | 19/11/2026 | 19/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — AWS Organizations<br>08 — Governance |
| Thứ Sáu | **Giám sát Trải nghiệm Người dùng (Frontend Observability)**<ul><li>Sử dụng trình duyệt Developer Tools (Network và Performance tab) để đo lường các chỉ số cốt lõi: Time to First Byte (TTFB), thời gian tải gói bundle JavaScript và độ trễ phản hồi của API.</li><li>Xây dựng các thành phần bắt lỗi (React Error Boundary): bắt các lỗi sập giao diện cục bộ, ngăn chặn màn hình trắng xóa (White Screen of Death) và hiển thị thông báo thân thiện cho người dùng.</li></ul> | 20/11/2026 | 20/11/2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>09 — AWS Health<br>10 — AWS Trusted Advisor |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Module 10 về Giám sát và Nhật ký mang lại cho em cái nhìn đa chiều về khái niệm Khả năng quan sát (Observability). Một ứng dụng web tốt không chỉ là code không có lỗi ở máy lập trình viên, mà phải có cơ chế theo dõi và cảnh báo liên tục khi vận hành thực tế.

Từ phía Frontend, em nhận thức rõ tầm quan trọng của việc xử lý lỗi duyên dáng (Graceful Error Handling). Khi API backend gặp sự cố hoặc trả về mã lỗi 500, thay vì để giao diện React bị đơ hoặc bung màn hình trắng xóa, em đã bọc các component trong Error Boundary và gắn kèm nút 'Thử lại'. Nhờ vậy, trải nghiệm của người dùng vẫn được duy trì ổn định ngay cả trong lúc hệ thống đang tự động hồi phục.

### Thành tựu Tuần 10

- Amazon CloudWatch là công cụ trung tâm để theo dõi chỉ số, gom log và gửi cảnh báo tự động khi hệ thống gặp bất thường.
- AWS CloudTrail cung cấp khả năng kiểm toán an ninh minh bạch cho mọi hành động thay đổi cấu hình trên tài khoản AWS.
- Áp dụng vào Tindy: Sử dụng DevTools Network để đo đạc thời gian phản hồi của API; xây dựng Error Boundary trong React để bắt lỗi và giữ cho giao diện luôn ổn định.
