---
title: "Nhật ký Công việc Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Module 11** — Kinh tế Đám mây, Lập Dự toán Chi phí (Pricing Calculator) và Tối ưu Ngân sách

### Mục tiêu Tuần 11

- Sử dụng công cụ AWS Pricing Calculator để lập bảng dự toán chi phí chi tiết cho toàn bộ kiến trúc ứng dụng web trước khi triển khai.
- Làm chủ các công cụ quản lý chi phí của AWS: AWS Cost Explorer, AWS Budgets và thiết lập ngưỡng cảnh báo ngân sách tự động.
- Xây dựng chiến lược tối ưu hóa tài nguyên cho môi trường thử nghiệm: tắt mở theo lịch trình (Resource Scheduling) để triệt tiêu chi phí nhàn rỗi.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Lập Dự toán Chi phí với AWS Pricing Calculator**<ul><li>Tìm hiểu công cụ AWS Pricing Calculator: mô hình hóa kiến trúc dự kiến và tính toán chi phí hàng tháng dựa trên nhu cầu sử dụng thực tế.</li><li>Thực hành cấu hình bảng dự toán cho Tindy: bao gồm dung lượng S3 tĩnh, băng thông CloudFront ra internet, 1 task ECS Fargate (0.25 vCPU, 0.5 GB RAM), 1 instance RDS PostgreSQL db.t4g.micro và số lượng token ước tính cho Amazon Bedrock.</li></ul> | 23/11/2026 | 23/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Pricing and Support<br>02 — AWS Pricing Concepts |
| Thứ Ba | **Phân tích Chi phí Thực tế với AWS Cost Explorer**<ul><li>Nghiên cứu công cụ AWS Cost Explorer: trực quan hóa chi phí phát sinh hàng ngày và hàng tháng dưới dạng biểu đồ cột chi tiết theo từng dịch vụ.</li><li>Khảo sát tính năng gắn nhãn tài nguyên (Cost Allocation Tags): gắn tag `Project: Tindy` và `Environment: Demo` để theo dõi và bóc tách chính xác chi phí của từng cấu phần dự án.</li></ul> | 24/11/2026 | 24/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Pricing and Billing Services |
| Thứ Tư | **Kiểm soát Ngân sách & Cảnh báo Chi phí với AWS Budgets**<ul><li>Khảo sát AWS Budgets: thiết lập hạn mức chi tiêu cố định cho tài khoản AWS trong kỳ thực tập (ví dụ: đặt hạn mức 15 USD/tháng).</li><li>Cấu hình quy tắc cảnh báo đa cấp: gửi email thông báo tự động khi chi phí thực tế chạm mốc 80% ngân sách hoặc khi chi phí dự báo cuối tháng có nguy cơ vượt 100% hạn mức.</li></ul> | 25/11/2026 | 25/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Support Plans |
| Thứ Năm | **Tận dụng Gói Miễn phí AWS Free Tier & Lựa chọn Mô hình Mua**<ul><li>Rà soát các chính sách của AWS Free Tier: 12 tháng miễn phí (RDS micro, EC2 t2.micro), miễn phí vĩnh viễn (Lambda 1 triệu request/tháng, CloudWatch 10 metrics), và dùng thử ngắn hạn.</li><li>So sánh việc sử dụng Fargate On-Demand so với Fargate Spot (tiết kiệm đến 70% chi phí cho các tác vụ kiểm thử có thể chịu gián đoạn ngắn).</li></ul> | 26/11/2026 | 26/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — AWS Marketplace and AWS Partners |
| Thứ Sáu | **Chiến lược Tối ưu Tài nguyên (Resource Scheduling)**<ul><li>Phân tích bài toán lãng phí tài nguyên: hệ thống demo chỉ cần chạy phục vụ chấm điểm và quay video trong giờ hành chính, việc để máy chủ chạy liên tục ban đêm gây lãng phí không cần thiết.</li><li>Thiết lập quy trình vận hành linh hoạt: chỉ bật container backend ECS và mở kết nối cơ sở dữ liệu khi tiến hành kiểm thử và quay video demo, sau đó tạm dừng để duy trì chi phí ở mức tối thiểu.</li></ul> | 27/11/2026 | 27/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Cost Optimization |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Trước khi tham gia chương trình thực tập này, em từng có nỗi sợ rằng việc sử dụng điện toán đám mây sẽ rất dễ phát sinh chi phí ngoài ý muốn. Tuần học về Kinh tế đám mây và Quản lý chi phí đã hoàn toàn xóa bỏ nỗi lo này của em.

Em hiểu rằng chi phí đám mây hoàn toàn nằm trong tầm kiểm soát nếu chúng ta biết cách lập dự toán trước bằng AWS Pricing Calculator và cài đặt cảnh báo qua AWS Budgets. Trong dự án Tindy, việc tách biệt phần Frontend tĩnh chạy trên S3/CloudFront (gần như miễn phí) với phần Backend chạy trên ECS Fargate đã giúp nhóm tối ưu hóa chi phí một cách xuất sắc: hệ thống chỉ tiêu tốn chưa đến vài USD cho toàn bộ quá trình phát triển và kiểm thử.

### Thành tựu Tuần 11

- AWS Pricing Calculator và AWS Budgets là hai công cụ không thể thiếu để lập kế hoạch tài chính và ngăn chặn chi phí phát sinh ngoài ý muốn.
- Tách rời frontend tĩnh (S3/CloudFront) và tối ưu hóa tài nguyên backend là chiến lược tiết kiệm chi phí hiệu quả nhất cho các ứng dụng web.
- Áp dụng vào Tindy: Lập bảng dự toán chi phí hàng tháng cho Tindy; thiết lập AWS Budgets gửi cảnh báo qua email để đảm bảo dự án luôn nằm trong hạn mức.
