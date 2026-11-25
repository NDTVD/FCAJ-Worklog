---
title: "Nhật ký Công việc Tuần 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Module 2** — EC2, điều phối lưu lượng và nhắn tin

### Mục tiêu Tuần 2

- Chọn loại Amazon EC2 instance và cách cấp phát dựa trên yêu cầu của workload.
- So sánh các lựa chọn mua EC2 và nêu vai trò của Auto Scaling, Elastic Load Balancing và health check.
- Giải thích cách dùng Amazon SQS và Amazon SNS để tách các thành phần ứng dụng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Vòng đời và các nhóm EC2 instance**<ul><li>Tìm hiểu ảo hóa và các trạng thái trong vòng đời EC2 instance. So sánh các nhóm instance theo nhu cầu CPU, bộ nhớ, tăng tốc phần cứng và lưu trữ.</li><li>Ghi lại các lựa chọn khi cấp phát EC2, gồm hệ điều hành, năng lực xử lý và ổ đĩa. So sánh trạng thái dừng với chấm dứt instance, rồi ghép nhóm instance phù hợp với ví dụ backend web thông thường, tác vụ CPU nặng và tác vụ cần nhiều bộ nhớ.</li></ul> | 21/09/2026 | 21/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Amazon EC2<br>02 — Amazon EC2 Instance Types |
| Thứ Ba | **Cấp phát tài nguyên và demo khởi tạo EC2**<ul><li>Đối chiếu AWS Management Console, AWS CLI, CloudShell và AWS SDK theo cách cấp phát và quản lý tài nguyên. Phân tích demo khởi tạo máy chủ web EC2 qua AMI, key pair, cấu hình mạng, EBS và user data.</li><li>Đặt cùng một tác vụ xem thông tin EC2 vào bối cảnh Console, CLI và SDK để giải thích khi nào dùng từng công cụ. Lần theo demo khởi tạo máy chủ và chú thích phần nào xác định phần mềm ban đầu, quyền kết nối, mạng, ổ đĩa và cấu hình lúc khởi động.</li></ul> | 22/09/2026 | 22/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — How to Provision AWS Resources<br>04 — Demo Launching an Amazon EC2 Instance |
| Thứ Tư | **Định giá Amazon EC2**<ul><li>So sánh On-Demand, Savings Plans, Reserved Instances, Spot Instances và Dedicated Hosts theo đặc điểm workload.</li><li>Lập bảng quyết định theo đặc điểm workload: thử nghiệm ngắn hạn, tải ổn định, tác vụ có thể gián đoạn và phần mềm có yêu cầu về máy chủ vật lý. Với mỗi tình huống, ghi lý do chọn mô hình mua và ràng buộc cần xem trước.</li></ul> | 23/09/2026 | 23/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon EC2 Pricing |
| Thứ Năm | **Mở rộng và cân bằng tải**<ul><li>Phân biệt mở rộng theo chiều dọc và chiều ngang. Tìm hiểu Auto Scaling group và vai trò của CloudWatch. Phân tích cách Elastic Load Balancing phân phối lưu lượng và dùng health check.</li><li>Mô tả cách ứng dụng xử lý đợt tăng tải. AWS Auto Scaling sẽ điều chỉnh công suất của nhóm EC2 trong khi cân bằng tải định tuyến các yêu cầu đến target đủ điều kiện. Vẽ thêm tình huống một target lỗi và chỉ ra vai trò của health check.</li></ul> | 24/09/2026 | 24/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Scaling Amazon EC2<br>07 — Directing Traffic with Elastic Load Balancing |
| Thứ Sáu | **Hàng đợi, thông báo và fanout**<ul><li>So sánh hàng đợi Amazon SQS và mô hình publish/subscribe của Amazon SNS qua ví dụ fanout.</li><li>Mô tả một producer gửi yêu cầu xử lý ảnh vào hàng đợi và một worker lấy việc ra xử lý. Mở rộng ví dụ thành mô hình fanout để một sự kiện được gửi tới nhiều hàng đợi, mỗi consumer xử lý tác vụ riêng. Ghi lý do dùng SNS và SQS ở từng điểm.</li></ul> | 25/09/2026 | 25/09/2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Messaging and Queuing |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Trong tuần học về Compute và Messaging, em đặc biệt chú ý đến cách thức Elastic Load Balancing (ALB) điều phối lưu lượng truy cập. Với vai trò Frontend phụ trách tính năng Chat thời gian thực trên Tindy, em nhận thấy ALB không chỉ đơn thuần phân chia HTTP request mà còn phải hỗ trợ duy trì kết nối WebSocket liên tục để người dùng không bị rớt kết nối SignalR khi đang nhắn tin.

Bên cạnh đó, việc tìm hiểu về Amazon SQS và SNS mang lại cho em tư duy thiết kế bất đồng bộ (asynchronous decoupling). Thay vì bắt người dùng phải chờ đợi trình duyệt xoay vòng khi upload tệp CV PDF nặng, hệ thống có thể tiếp nhận yêu cầu ngay lập tức và đẩy tác vụ quét virus, trích xuất AI vào hàng đợi ngầm phía sau, giúp tối ưu hóa đáng kể trải nghiệm tương tác (UX) của người dùng.

### Thành tựu Tuần 2

- Loại instance phụ thuộc vào nhu cầu của workload. AMI xác định phần mềm ban đầu, còn user data có thể chạy các bước cấu hình khi khởi tạo.
- EC2 Auto Scaling điều chỉnh số lượng instance, Elastic Load Balancing phân phối yêu cầu, còn SQS và SNS hỗ trợ giao tiếp bất đồng bộ.
- **Áp dụng vào Tindy:** Hiểu cách Application Load Balancer (ALB) điều phối lưu lượng và duy trì kết nối WebSocket liên tục cho khung chat SignalR hai chiều.


