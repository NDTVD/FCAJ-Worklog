---
title: "Nhật ký Công việc Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Module 3** — Điện toán Không Máy chủ (Serverless) và Điều phối Container

### Mục tiêu Tuần 3

- Nắm vững nguyên lý hoạt động của kiến trúc Serverless với AWS Lambda và cơ chế kích hoạt theo sự kiện (Event-driven).
- Hiểu rõ công nghệ Container hóa (Docker) và cách lưu trữ image trên Amazon Elastic Container Registry (ECR).
- So sánh các nền tảng điều phối container Amazon ECS và Amazon EKS; phân tích lợi thế vận hành không máy chủ của AWS Fargate.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Khảo sát Kiến trúc Serverless với AWS Lambda**<ul><li>Tìm hiểu bản chất Serverless: không cần quản trị máy chủ, tự động co giãn theo từng request, và chỉ trả tiền khi code thực thi (tính theo mili-giây).</li><li>Phân tích các nguồn kích hoạt Lambda: HTTP request qua API Gateway, sự kiện upload tệp trên S3, hoặc thông điệp mới trong hàng đợi SQS. Tìm hiểu giới hạn thời gian chạy (Execution timeout 15 phút) và quản lý Cold Start.</li></ul> | 28/09/2026 | 28/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Serverless Computing |
| Thứ Ba | **Công nghệ Container & Quản lý Image với Amazon ECR**<ul><li>So sánh sự khác biệt giữa Máy ảo (Virtual Machines) và Container: Container chia sẻ chung nhân hệ điều hành (OS Kernel), dung lượng nhẹ hơn và thời gian khởi động tính bằng giây.</li><li>Tìm hiểu Amazon Elastic Container Registry (ECR): tạo repository riêng tư, gắn thẻ (tagging) image theo digest git commit SHA, và thiết lập quyền truy cập cho pipeline CI/CD đẩy image lên an toàn.</li></ul> | 29/09/2026 | 29/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda |
| Thứ Tư | **Điều phối Container với Amazon ECS và Amazon EKS**<ul><li>Khảo sát Amazon Elastic Container Service (ECS) - giải pháp điều phối container tối giản, tích hợp sâu vào hệ sinh thái AWS.</li><li>So sánh Amazon ECS với Amazon Elastic Kubernetes Service (EKS) cho các ứng dụng đòi hỏi chuẩn Kubernetes mã nguồn mở. Tìm hiểu khái niệm ECS Task Definition (khai báo CPU, RAM, cổng mạng, biến môi trường) và ECS Service (duy trì số lượng bản sao mong muốn).</li></ul> | 30/09/2026 | 30/09/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Containers and Orchestration on AWS |
| Thứ Năm | **Vận hành Container Không Máy chủ với AWS Fargate**<ul><li>Phân tích sự khác biệt giữa việc tự quản lý EC2 Launch Type và sử dụng AWS Fargate Serverless Launch Type trong ECS.</li><li>Tìm hiểu cách Fargate tự động cấp phát tài nguyên hạ tầng bên dưới: lập trình viên chỉ cần chỉ định lượng vCPU và RAM cần thiết cho container, AWS sẽ đảm nhận toàn bộ việc vá lỗi hệ điều hành và bảo trì máy chủ vật lý.</li></ul> | 01/10/2026 | 01/10/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Additional Compute Services |
| Thứ Sáu | **Mô hình Hóa Ứng dụng Web Đa Tầng trên Container**<ul><li>Vẽ sơ đồ kiến trúc ứng dụng web: frontend tĩnh tải từ S3/CloudFront, API nghiệp vụ đóng gói thành container chạy trên ECS Fargate sau Application Load Balancer.</li><li>Phân tích cách cấu hình biến môi trường nhạy cảm (Connection String, JWT Secrets) truyền vào ECS task definition mà không bị lộ trong mã nguồn.</li></ul> | 02/10/2026 | 02/10/2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda<br>03 — Containers and Orchestration on AWS<br>04 — Additional Compute Services |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần này em tìm hiểu sâu về Docker, Amazon ECR và Amazon ECS Fargate. Đây là những khái niệm vô cùng thực tế giúp em kết nối quá trình code ở local với môi trường chạy thực tế trên Cloud. Trước đây em thường chạy backend ASP.NET Core trực tiếp bằng Visual Studio hoặc dotnet CLI; qua module này, em hiểu cách toàn bộ backend được đóng gói thành một Docker container hoàn chỉnh, đẩy lên ECR và vận hành tự động bởi ECS Fargate mà không cần tự cấu hình từng máy chủ EC2.

Khái niệm serverless của Fargate rất ấn tượng: tài nguyên chỉ được cấp phát chính xác theo lượng CPU và RAM mà container yêu cầu. Điều này giúp em và nhóm giải quyết được bài toán cân đối chi phí trong các đợt chạy thử nghiệm và demo dự án.

### Thành tựu Tuần 3

- Serverless và Container là hai xu hướng công nghệ hàng đầu giúp tối ưu hóa chu kỳ phát hành phần mềm và tiết kiệm chi phí.
- AWS Fargate loại bỏ hoàn toàn gánh nặng quản lý máy chủ ảo, giúp lập trình viên tập trung 100% vào mã nguồn ứng dụng.
- Áp dụng vào Tindy: Nắm rõ cách đóng gói backend ASP.NET Core thành Docker image lưu trên ECR và vận hành container không máy chủ qua ECS Fargate.
