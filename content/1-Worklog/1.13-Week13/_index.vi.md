---
title: "Nhật ký Công việc Tuần 13"
date: 2024-01-01
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

**Module 13** — AWS Well-Architected và tổng kết thực tập

### Mục tiêu Tuần 13

- Áp dụng sáu trụ cột của AWS Well-Architected Framework để đánh giá một workload.
- Giải thích khi nào dùng dịch vụ AWS chuyên dụng qua các tình huống kiến trúc của khóa học.
- Liên hệ các điểm đánh đổi trong kiến trúc Tindy với nội dung đã học và hoàn thiện hồ sơ tổng kết.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Từ hệ thống chạy được đến đánh giá kiến trúc**<ul><li>Đọc sơ đồ Tindy và chia theo lối vào CloudFront, lớp tính toán ECS Fargate, cơ sở dữ liệu PostgreSQL và luồng tài liệu trên S3.</li><li>Đặt câu hỏi về khả năng phục hồi, bảo mật và vận hành cho từng lớp. Dùng cấu hình demo làm ví dụ để ghi rõ giả định về số người sử dụng, thời gian chạy và mức gián đoạn có thể chấp nhận.</li></ul> | 07/12/2026 | 07/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions |
| Thứ Ba | **Dịch vụ AWS chuyên dụng**<ul><li>Ghép CodePipeline với điều phối CI/CD, X-Ray với truy vết phân tán, AppSync với API GraphQL và Amplify với công việc phát triển ứng dụng web.</li><li>Đối chiếu Amazon SES và Amazon Connect theo nhu cầu email hoặc trung tâm liên hệ. Phân biệt các ví dụ phân phối ứng dụng, desktop và truy cập web quản lý tập trung trong bài dựa trên công việc người dùng cần thực hiện.</li></ul> | 08/12/2026 | 08/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Specialized Services |
| Thứ Tư | **Sáu trụ cột AWS Well-Architected**<ul><li>Lập bảng sáu trụ cột gồm Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization và Sustainability. Gắn mỗi trụ cột với một câu hỏi cho ứng dụng.</li><li>Phân biệt Framework cung cấp tiêu chí với Well-Architected Tool hỗ trợ ghi nhận đánh giá. Xem cách ưu tiên rủi ro theo ảnh hưởng, ghi bằng chứng và đề xuất việc cần kiểm chứng ở lần đánh giá sau.</li></ul> | 09/12/2026 | 09/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Well-Architected Framework |
| Thứ Năm | **Ba tình huống kiến trúc chuyên biệt**<ul><li>Lần theo yêu cầu trong backend serverless qua API Gateway, Lambda và DynamoDB. Xác định nơi cần quan sát lỗi hoặc độ trễ bằng log và truy vết.</li><li>So sánh với website tĩnh trên S3 có biểu mẫu gửi email qua SES và trung tâm liên hệ dùng Amazon Connect có nhiều kênh hoặc callback. Nêu phần nào của quy trình mỗi dịch vụ đảm nhiệm.</li></ul> | 10/12/2026 | 10/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Specialized Use Cases |
| Thứ Sáu | **Rà soát kiến trúc Tindy và tổng hợp kiến thức**<ul><li>Dùng sáu trụ cột để rà cấu hình demo Tindy. Đối chiếu giới hạn của một Fargate task và RDS Single-AZ với cách giám sát readiness, lưu bản sao lưu và khôi phục sau sự cố.</li><li>Phân loại những gì mã nguồn hoặc tài liệu đã mô tả và những gì cần xác minh thêm. Chuẩn bị danh sách mục tiêu, bằng chứng và nguồn trích dẫn để hoàn thiện báo cáo Việt–Anh.</li></ul> | 11/12/2026 | 11/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions<br>03 — AWS Well-Architected Framework<br>04 — Specialized Use Cases |
| Thứ Hai | **Tổng kết thực tập**<ul><li>Tổng kết thực tập và hoàn thiện báo cáo.</li><li>Chốt phần tự đánh giá dựa trên kiến thức và công việc đã ghi nhận. Rà lần cuối mục lục, nội dung Việt–Anh và nguồn của từng minh chứng trước khi hoàn thiện báo cáo.</li></ul> | 14/12/2026 | 14/12/2026 | Báo cáo thực tập |

### Thành tựu Tuần 13

- Sáu trụ cột cung cấp tiêu chí đánh giá kiến trúc. Well-Architected Tool hỗ trợ ghi nhận câu trả lời, rủi ro và việc cải tiến.
- Có thể giải thích vai trò của dịch vụ chuyên dụng qua ba luồng mẫu: backend serverless, biểu mẫu liên hệ và contact center.
- Phần tổng kết liên hệ bối cảnh demo Tindy với các quyết định về bảo mật, độ tin cậy, vận hành và chi phí.
- **Áp dụng vào Tindy:** Đánh giá kiến trúc Tindy theo 6 trụ cột Well-Architected; hoàn thiện kịch bản kiểm thử giao diện và nghiệm thu Workshop 5.6.

