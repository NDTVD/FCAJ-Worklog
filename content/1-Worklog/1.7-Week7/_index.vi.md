---
title: "Nhật ký Công việc Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Module 7** — Cơ sở Dữ liệu Đám mây (RDS PostgreSQL, DynamoDB) và Bộ nhớ Đệm

### Mục tiêu Tuần 7

- So sánh sự khác biệt cốt lõi giữa Cơ sở dữ liệu quan hệ (Relational - RDS) và phi quan hệ (NoSQL - DynamoDB).
- Hiểu rõ các tính năng đảm bảo độ sẵn sàng cao của Amazon RDS: Multi-AZ Deployment, Read Replicas và Automated Backups.
- Nắm bắt kỹ thuật tối ưu hóa truy vấn dữ liệu từ phía Frontend: phân trang (Pagination), lọc dữ liệu và áp dụng bộ nhớ đệm (Caching).

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Cơ sở Dữ liệu Quan hệ với Amazon RDS PostgreSQL**<ul><li>Khảo sát dịch vụ Amazon Relational Database Service (RDS): tự động hóa việc cấp phát phần cứng, cài đặt hệ quản trị, vá lỗi bảo mật định kỳ và sao lưu tự động.</li><li>Phân tích cấu trúc dữ liệu quan hệ cho Tindy: bảng Users, Projects, Applications, Messages với các ràng buộc khóa ngoại (Foreign Keys) đảm bảo tính toàn vẹn dữ liệu ACID.</li></ul> | 26/10/2026 | 26/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Databases |
| Thứ Ba | **Tính Sẵn sàng Cao (Multi-AZ) & Mở rộng Đọc (Read Replicas)**<ul><li>Nghiên cứu cơ chế Multi-AZ Deployment: tự động đồng bộ dữ liệu sang một Standby Instance ở Availability Zone khác, tự động chuyển đổi dự phòng (failover) trong vài phút khi có sự cố.</li><li>Tìm hiểu Read Replicas: tạo các bản sao bất đồng bộ để chia sẻ tải đọc cho các truy vấn tìm kiếm dự án và danh sách ứng viên, giảm áp lực cho máy chủ ghi chính.</li></ul> | 27/10/2026 | 27/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Relational Database Services |
| Thứ Tư | **Cơ sở Dữ liệu Phi Quan hệ NoSQL với Amazon DynamoDB**<ul><li>Khảo sát kiến trúc NoSQL của Amazon DynamoDB: mô hình dữ liệu Key-Value và Document, cung cấp độ trễ ổn định ở mức một chữ số mili-giây ở bất kỳ quy mô nào.</li><li>Phân tích cách chọn Partition Key (PK) và Sort Key (SK) để tối ưu hóa việc truy vấn dữ liệu lịch sử chat, thông báo và trạng thái online/offline của người dùng.</li></ul> | 28/10/2026 | 28/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — NoSQL Database Services |
| Thứ Năm | **Tăng tốc Truy vấn với Bộ nhớ Đệm Amazon ElastiCache (Redis)**<ul><li>Tìm hiểu chiến lược lưu đệm Cache-Aside: lưu trữ các dữ liệu ít biến động nhưng tần suất đọc cực cao (danh mục kỹ năng, dự án nổi bật) trên RAM với độ trễ micro-giây.</li><li>Khảo sát cơ chế hết hạn thời gian (TTL - Time to Live) và cách xóa đệm (Cache Invalidation) để đảm bảo dữ liệu hiển thị trên giao diện không bị sai lệch quá lâu.</li></ul> | 29/10/2026 | 29/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Databases Demonstration |
| Thứ Sáu | **Tối ưu Hóa Truy xuất Dữ liệu Phía Frontend (Client Fetching)**<ul><li>Nghiên cứu các phương pháp phân trang: Phân trang theo số trang (Offset/Limit) và Phân trang theo con trỏ (Cursor-based Pagination) để tránh tải dồn dập hàng nghìn bản ghi lên trình duyệt.</li><li>Xây dựng các trạng thái giao diện: hiển thị Skeleton loading mượt mà trong khi chờ API phản hồi, xử lý trạng thái rỗng (Empty State) và thông báo lỗi kết nối cơ sở dữ liệu.</li></ul> | 30/10/2026 | 30/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — In-Memory Caching Services<br>06 — Additional Database Services |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Trước đây em thường cho rằng việc cơ sở dữ liệu chạy nhanh hay chậm hoàn toàn phụ thuộc vào người viết câu lệnh SQL ở backend. Tuy nhiên, qua Module 7, em hiểu rằng cách lập trình viên Frontend thiết kế giao diện và gọi API có ảnh hưởng trực tiếp đến hiệu năng của cơ sở dữ liệu.

Nếu giao diện React cứ mỗi lần người dùng gõ phím lại gửi một request tìm kiếm mà không có cơ chế `debounce`, hoặc tải toàn bộ danh sách 10.000 dự án cùng lúc mà không có phân trang, cơ sở dữ liệu sẽ bị quá tải ngay lập tức. Em đã chủ động áp dụng kỹ thuật Debounce và Infinite Scrolling phân trang trên giao diện Tindy để bảo vệ cơ sở dữ liệu PostgreSQL phía sau.

### Thành tựu Tuần 7

- Amazon RDS PostgreSQL cung cấp độ tin cậy giao dịch ACID cao, trong khi Multi-AZ đảm bảo hệ thống không bị sập nguồn dữ liệu.
- Áp dụng bộ nhớ đệm (Caching) và phân trang là chìa khóa để giảm tải cho cơ sở dữ liệu và duy trì tốc độ phản hồi nhanh.
- Áp dụng vào Tindy: Lập trình giao diện tìm kiếm dự án với cơ chế Debounce và phân trang dữ liệu, giảm thiểu số lượng truy vấn đè nặng lên RDS PostgreSQL.
