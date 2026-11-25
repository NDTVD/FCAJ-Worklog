---
title: "Nhật ký Công việc Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Module 3** — Serverless, container và dịch vụ compute

### Mục tiêu Tuần 3

- So sánh trách nhiệm vận hành giữa EC2, dịch vụ được quản lý và serverless.
- Giải thích luồng xử lý sự kiện của AWS Lambda, gồm trigger, handler và quyền thực thi.
- Chọn container hoặc dịch vụ compute chuyên biệt theo yêu cầu triển khai và đặc điểm tác vụ.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Serverless và trách nhiệm vận hành**<ul><li>So sánh EC2, dịch vụ được quản lý và serverless theo mức độ kiểm soát hạ tầng và công việc vận hành.</li><li>So sánh các việc vận hành còn lại khi chạy ứng dụng trên EC2 với khi dùng dịch vụ được quản lý hoặc serverless. Lập một bảng ngắn cho các việc như quản lý máy chủ, mở rộng công suất, triển khai mã và cấu hình quyền ứng dụng.</li></ul> | 28/09/2026 | 28/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Serverless Computing |
| Thứ Ba | **Xử lý sự kiện với AWS Lambda**<ul><li>Phân tích trigger, event, handler và quyền thực thi của Lambda qua ví dụ xử lý tệp tải lên S3.</li><li>Lần theo một lần tải tệp lên S3. Xác định nguồn sự kiện, dữ liệu chuyển cho hàm, phần mã xử lý và quyền cần thiết nếu hàm phải đọc hoặc ghi dữ liệu. Ghi xem thời lượng xử lý ảnh hưởng thế nào đến quyết định dùng Lambda.</li></ul> | 29/09/2026 | 29/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda |
| Thứ Tư | **Container và điều phối**<ul><li>Phân biệt container và máy ảo. Tìm hiểu vai trò của Amazon ECS, Amazon EKS, Amazon ECR và AWS Fargate.</li><li>Đặt cùng một ứng dụng vào hai mô hình máy ảo và container để so sánh cách đóng gói và nhất quán giữa môi trường. Vẽ luồng từ image trong ECR đến container do ECS hoặc EKS điều phối, rồi chú thích lựa chọn chạy trên EC2 hoặc Fargate.</li></ul> | 30/09/2026 | 30/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Containers and Orchestration on AWS |
| Thứ Năm | **Các dịch vụ compute bổ sung**<ul><li>Đối chiếu AWS Elastic Beanstalk, AWS Batch, Amazon Lightsail và AWS Outposts theo tình huống sử dụng.</li><li>Lập danh sách bốn nhu cầu: triển khai web app, chạy batch job, thuê máy chủ đơn giản và vận hành hạ tầng AWS tại chỗ. Ghép từng nhu cầu với dịch vụ trong bài và nêu phần việc đội ứng dụng vẫn phải quản lý.</li></ul> | 01/10/2026 | 01/10/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Additional Compute Services |
| Thứ Sáu | **Ôn tập qua tình huống chọn dịch vụ**<ul><li>Ôn Module 3 bằng ba tình huống: xử lý tệp tải lên, chạy ứng dụng đóng gói container và xử lý tác vụ theo lô. Chọn dịch vụ và giải thích lý do.</li><li>Với mỗi tình huống ôn tập, ghi rõ thời lượng công việc, đầu vào và nhu cầu kiểm soát môi trường. Chọn một phương án compute, giải thích lý do và nêu giả định có thể làm thay đổi lựa chọn. Dùng tình huống xử lý tệp để chuẩn bị cho lab Lambda.</li></ul> | 02/10/2026 | 02/10/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda<br>03 — Containers and Orchestration on AWS<br>04 — Additional Compute Services |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần này em tìm hiểu sâu về Docker, Amazon ECR và Amazon ECS Fargate. Đây là những khái niệm vô cùng thực tế giúp em kết nối quá trình code ở local với môi trường chạy thực tế trên Cloud. Trước đây em thường chạy backend ASP.NET Core trực tiếp bằng Visual Studio hoặc dotnet CLI; qua module này, em hiểu cách toàn bộ backend được đóng gói thành một Docker container hoàn chỉnh, đẩy lên ECR và vận hành tự động bởi ECS Fargate mà không cần tự cấu hình từng máy chủ EC2.

Khái niệm serverless của Fargate rất ấn tượng: tài nguyên chỉ được cấp phát chính xác theo lượng CPU và RAM mà container yêu cầu. Điều này giúp em và nhóm giải quyết được bài toán cân đối chi phí trong các đợt chạy thử nghiệm và demo dự án.

### Thành tựu Tuần 3

- Lambda phù hợp với tác vụ theo sự kiện. Thời lượng xử lý và quyền thực thi là hai yếu tố cần xem khi chọn Lambda.
- ECR lưu container image, ECS và EKS điều phối container, còn Fargate cung cấp năng lực chạy container.
- **Áp dụng vào Tindy:** Nắm rõ cách đóng gói backend ASP.NET Core thành Docker image lưu trên ECR và vận hành container không máy chủ qua ECS Fargate.


