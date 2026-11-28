---
title: "Nhật ký Công việc Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

**Module 1** — Nền tảng Điện toán Đám mây và Hạ tầng Toàn cầu AWS

### Mục tiêu Tuần 1

- Hiểu rõ bản chất mô hình Client–Server, cơ chế tính phí Pay-as-you-go và sự khác biệt giữa hạ tầng tại chỗ (On-premises) với điện toán đám mây.
- Phân tích cấu trúc phân cấp hạ tầng toàn cầu của AWS: Region, Availability Zone (AZ) và Data Center để đưa ra quyết định đặt tài nguyên tối ưu.
- Nắm vững Mô hình Trách nhiệm Chia sẻ (AWS Shared Responsibility Model) để xác định rõ ranh giới bảo mật của nhà cung cấp và đội ngũ phát triển ứng dụng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Nguyên lý Điện toán Đám mây & Kiến trúc Client–Server**<ul><li>Khảo sát cơ chế tương tác Client–Server: trình duyệt web đóng vai trò client gửi request qua Internet và nhận response từ server.</li><li>So sánh chi phí đầu tư ban đầu (CAPEX) khi mua máy chủ vật lý với chi phí vận hành linh hoạt (OPEX) trên đám mây. Đánh giá tính co giãn giúp hệ thống tự động thích ứng với lượng truy cập biến động.</li></ul> | 14/09/2026 | 14/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01–02 — Welcome to AWS Cloud Practitioner Essentials<br>What is Cloud Computing |
| Thứ Ba | **Phân tích 6 Lợi ích Cốt lõi của AWS Cloud**<ul><li>Tổng hợp và chứng minh 6 lợi thế lớn: chuyển đổi vốn đầu tư cố định thành chi phí biến đổi, tận dụng lợi thế kinh tế nhờ quy mô, ngừng phỏng đoán dung lượng, tăng tốc độ triển khai phần mềm, giải phóng nguồn lực khỏi việc bảo trì trung tâm dữ liệu, và khả năng mở rộng quy mô toàn cầu chỉ sau vài phút.</li><li>Đặt vào kịch bản thực tế của ứng dụng tuyển dụng sinh viên Tindy khi có lượng đăng ký tăng đột biến đầu học kỳ.</li></ul> | 15/09/2026 | 15/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Benefits of the AWS Cloud |
| Thứ Tư | **Cấu trúc Hạ tầng Toàn cầu của AWS**<ul><li>Tìm hiểu sâu về cấu trúc Region và Availability Zone. Một AWS Region chuẩn luôn bao gồm từ 3 AZ biệt lập trở lên nhằm loại bỏ điểm lỗi đơn lẻ (Single Point of Failure).</li><li>Phân tích kịch bản ứng dụng triển khai Multi-AZ: khi một Availability Zone gặp sự cố gián đoạn nguồn điện hoặc cáp quang, lưu lượng mạng sẽ tự động chuyển hướng sang AZ còn lại mà người dùng không bị gián đoạn dịch vụ.</li></ul> | 16/09/2026 | 16/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to AWS Global Infrastructure |
| Thứ Năm | **Mô hình Trách nhiệm Chia sẻ trong Bảo mật Đám mây**<ul><li>Nghiên cứu nguyên tắc phân định: AWS chịu trách nhiệm 'Security OF the Cloud' (bảo vệ phần cứng, trung tâm dữ liệu và lớp ảo hóa), còn Khách hàng chịu trách nhiệm 'Security IN the Cloud' (bảo mật hệ điều hành, dữ liệu người dùng, phân quyền truy cập IAM và mã nguồn ứng dụng).</li><li>Đối chiếu mức độ trách nhiệm của lập trình viên khi sử dụng máy chủ ảo EC2 so với cơ sở dữ liệu quản lý RDS và dịch vụ lưu trữ tĩnh S3.</li></ul> | 17/09/2026 | 17/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — The AWS Shared Responsibility Model |
| Thứ Sáu | **Mô phỏng Thiết kế Hệ thống Thực tế**<ul><li>Thực hành thiết kế kiến trúc mức cao cho một nền tảng web phục vụ người dùng sinh viên. Đánh giá tiêu chí chọn Region dựa trên độ trễ địa lý và chi phí dịch vụ.</li><li>Phác thảo mô hình phân bổ tài nguyên: tách biệt thành phần giao diện tĩnh (Frontend Static Assets) với các endpoint API xử lý nghiệp vụ động nhằm tối ưu hóa tính sẵn sàng cao.</li></ul> | 18/09/2026 | 18/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Applying Cloud Concepts to Real Life Use Cases |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Là một lập trình viên chuyên tâm về Frontend (React / TypeScript), trước đây em thường chỉ quan tâm đến những gì diễn ra trong phạm vi trình duyệt: cách render component, quản lý state và xử lý sự kiện giao diện. Khi bước vào Tuần 1 của chương trình FCAJ, em nhận ra rằng một giao diện dù tối ưu mượt mà đến đâu cũng không thể mang lại trải nghiệm tốt nếu hạ tầng máy chủ phía sau chậm chạp hoặc gặp sự cố.

Việc phân tích mô hình Client–Server và Hạ tầng toàn cầu AWS giúp em hiểu rõ con đường dữ liệu đi từ trình duyệt người dùng đến máy chủ. Đặc biệt, mô hình trách nhiệm chia sẻ đã thay đổi tư duy của em: việc bảo vệ dữ liệu ở phía Client, không để lộ API key trong mã nguồn React và cấu hình các chính sách CORS an toàn chính là trách nhiệm trực tiếp của em chứ không thể phó mặc cho nhà cung cấp đám mây.

### Thành tựu Tuần 1

- Điện toán đám mây giúp chuyển đổi chi phí cố định thành chi phí biến đổi linh hoạt, giải phóng lập trình viên khỏi gánh nặng quản lý phần cứng.
- Thiết kế phân bổ trên nhiều Availability Zone (Multi-AZ) là tiêu chuẩn bắt buộc để đảm bảo ứng dụng web luôn hoạt động liên tục.
- Áp dụng vào Tindy: Phân tích luồng Client–Server giữa React Frontend (Vite) và API ASP.NET Core; tìm hiểu cơ chế trả phí theo nhu cầu thực tế để kiểm soát chi phí cho các tài nguyên demo.
