---
title: "Nhật ký Công việc Tuần 13"
date: 2024-01-01
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

**Module 13** — Khung Kiến trúc Chuẩn AWS Well-Architected và Tổng kết Kỳ Thực tập

### Mục tiêu Tuần 13

- Làm chủ 6 Trụ cột của AWS Well-Architected Framework: Vận hành Xuất sắc, Bảo mật, Độ tin cậy, Hiệu quả Hiệu năng, Tối ưu Chi phí và Tính Bền vững.
- Sử dụng công cụ AWS Well-Architected Tool để rà soát, đánh giá rủi ro và xác định các điểm cải tiến cho toàn bộ hệ thống Tindy.
- Tổng kết toàn diện kết quả thực tập cá nhân, nghiệm thu video demo ứng dụng thực tế và hoàn thiện báo cáo thực tập song ngữ.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Rà soát Kiến trúc Toàn diện Hệ thống Tindy**<ul><li>Phân tích sơ đồ kiến trúc hoàn chỉnh của Tindy: phân tầng rõ rệt từ CloudFront CDN phân phối giao diện tĩnh, Application Load Balancer tiếp nhận request API, ECS Fargate thực thi backend container, RDS PostgreSQL lưu trữ dữ liệu bền vững, và S3 lưu trữ tệp CV.</li><li>Kiểm tra tính chịu lỗi và các điểm đơn lỗi (Single Point of Failure) trên từng lớp kiến trúc; ghi nhận các giả định về lượng người dùng đồng thời và thời gian phục hồi sau sự cố.</li></ul> | 07/12/2026 | 07/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions |
| Thứ Ba | **Khảo sát Các Dịch vụ Chuyên biệt Bổ trợ của AWS**<ul><li>Tìm hiểu các dịch vụ đám mây nâng cao: AWS X-Ray (truy vết phân tán phân tích độ trễ microservices), AWS AppSync (quản lý GraphQL API thời gian thực), và AWS Amplify (nền tảng phát triển nhanh ứng dụng web/mobile).</li><li>Khảo sát Amazon SES (dịch vụ gửi email thông báo tự động) và Amazon Connect (tổng đài chăm sóc khách hàng đám mây); so sánh với kiến trúc hiện tại của dự án.</li></ul> | 08/12/2026 | 08/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Specialized Services |
| Thứ Tư | **6 Trụ cột của AWS Well-Architected Framework**<ul><li>Nghiên cứu chi tiết 6 trụ cột: 1) Vận hành Xuất sắc (tự động hóa phát hành qua CI/CD); 2) Bảo mật (phân quyền IAM, mã hóa dữ liệu, cấu hình CORS); 3) Độ tin cậy (Multi-AZ, Auto Scaling); 4) Hiệu quả Hiệu năng (CloudFront CDN, RDS Read Replicas); 5) Tối ưu Chi phí (Fargate serverless, S3 Lifecycle); 6) Tính Bền vững (giảm tài nguyên nhàn rỗi).</li><li>Thực hành sử dụng công cụ AWS Well-Architected Tool để đối chiếu hệ thống và tạo danh sách các hành động cần cải tiến (Workload Review).</li></ul> | 09/12/2026 | 09/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Well-Architected Framework |
| Thứ Năm | **Phân tích Các Tình huống Thiết kế Kiến trúc Chuyên sâu**<ul><li>Khảo sát mô hình kiến trúc Serverless thuần túy (API Gateway kết hợp AWS Lambda và DynamoDB); phân tích các điểm đánh đổi về độ trễ Cold Start và chi phí so với kiến trúc Container trên ECS Fargate.</li><li>Đánh giá kịch bản kết hợp giữa trang web tĩnh trên S3 với dịch vụ xử lý nền bất đồng bộ qua hàng đợi SQS để phục vụ bài toán mở rộng quy mô lớn.</li></ul> | 10/12/2026 | 10/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Specialized Use Cases |
| Thứ Sáu | **Nghiệm thu Hệ thống & Kiểm thử Kịch bản Demo Ứng dụng**<ul><li>Tiến hành kiểm thử luồng tương tác thực tế từ đầu đến cuối trên môi trường CloudFront chính thức: Onboarding tài khoản, tạo và đăng bài tuyển dụng, tìm kiếm cơ hội và ứng tuyển, nhắn tin trao đổi thời gian thực, và quét CV bằng Bedrock trong AI Studio.</li><li>Kiểm tra video demo ứng dụng (thời lượng 7 phút 22 giây), đối chiếu các khung hình chụp bằng chứng và xác minh sự ổn định của hệ thống trước khi nghiệm thu.</li></ul> | 11/12/2026 | 11/12/2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions<br>03 — AWS Well-Architected Framework<br>04 — Specialized Use Cases |
| Thứ Hai (14/12) | **Tổng kết Kỳ Thực tập & Hoàn thiện Báo cáo Song ngữ**<ul><li>Hoàn thiện hồ sơ thực tập cá nhân: cập nhật đầy đủ nhật ký công việc 13 tuần, phần tự đánh giá bản thân (Self-Evaluation) và chia sẻ phản hồi (Reflections and Feedback) mang đậm dấu ấn cá nhân Cao Thành Nhân.</li><li>Rà soát toàn bộ các mục báo cáo song ngữ (Anh - Việt), đảm bảo các tài liệu tóm tắt dự án (Markdown và XML draw.io) đã sẵn sàng để nộp bài đúng hạn.</li></ul> | 14/12/2026 | 14/12/2026 | Internship report |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần thứ 13 khép lại kỳ thực tập Workforce Bootcamp - First Cloud AI Journey đầy ý nghĩa. Nhìn lại chặng đường từ những ngày đầu còn bỡ ngỡ với các khái niệm IAM, VPC, EC2 đến nay em đã có thể tự tin tham gia xây dựng và vận hành một sản phẩm web hoàn chỉnh như Tindy trên hạ tầng AWS chuẩn mực.

Việc đối chiếu hệ thống với 6 trụ cột của AWS Well-Architected Framework giúp em hình thành tư duy kiến trúc toàn diện: một lập trình viên giỏi không chỉ biết viết code chạy được, mà phải hiểu rõ mã nguồn của mình vận hành trên môi trường nào, độ an toàn ra sao, chi phí bao nhiêu và có thể mở rộng được không. Những trải nghiệm thực tế với React, TypeScript, CORS, Rate Limiting và AWS Cloud chính là hành trang quý báu nhất cho sự nghiệp kỹ sư phần mềm của em.

### Thành tựu Tuần 13

- Khung Well-Architected với 6 trụ cột là kim chỉ nam hàng đầu để thiết kế, đánh giá và hoàn thiện các hệ thống đám mây đạt chuẩn doanh nghiệp.
- Kỳ thực tập đã giúp em nâng cao toàn diện kỹ năng lập trình web hiện đại kết hợp với tư duy kiến trúc đám mây thực chiến.
- Áp dụng vào Tindy: Đối chiếu Tindy theo 6 trụ cột Well-Architected; hoàn tất nghiệm thu video demo 5.6 và toàn bộ báo cáo thực tập song ngữ.
