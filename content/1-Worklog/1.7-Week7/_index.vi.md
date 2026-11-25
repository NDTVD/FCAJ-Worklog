---
title: "Nhật ký Công việc Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Module 7** — Cơ sở dữ liệu và bộ nhớ đệm trên AWS

### Mục tiêu Tuần 7

- Chọn cơ sở dữ liệu quan hệ hoặc NoSQL dựa trên mô hình dữ liệu, giao dịch và mẫu truy cập.
- Phân tích thao tác SQL và DynamoDB trong bài demo của khóa học.
- Giải thích vai trò của cache, cơ sở dữ liệu chuyên dụng và sao lưu.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Chọn cơ sở dữ liệu theo bài toán**<ul><li>Dùng chương trình tích điểm của quán cà phê để xác định dữ liệu khách hàng, giao dịch và số điểm cần lưu.</li><li>Liệt kê các thao tác đọc và ghi thường gặp trước khi chọn dịch vụ. Liên hệ với Tindy qua các quan hệ giữa tài khoản, dự án và đơn ứng tuyển, rồi giải thích vì sao mẫu truy cập ảnh hưởng đến thiết kế dữ liệu.</li></ul> | 26/10/2026 | 26/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Databases |
| Thứ Ba | **SQL, Amazon RDS và Amazon Aurora**<ul><li>Ôn bảng, khóa chính, khóa ngoại và giao dịch SQL. Dùng thao tác cập nhật hồ sơ tuyển dụng để phân tích vì sao nhiều thay đổi liên quan cần nhất quán.</li><li>So sánh tự vận hành cơ sở dữ liệu trên EC2 với Amazon RDS và Aurora. Ghi rõ phần việc ứng dụng vẫn quản lý, gồm schema và quyền truy cập, rồi đọc cách bản sao lưu và khôi phục tại một thời điểm hỗ trợ vận hành.</li></ul> | 27/10/2026 | 27/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Relational Database Services |
| Thứ Tư | **Amazon DynamoDB và mẫu truy cập NoSQL**<ul><li>Phân biệt table, item và attribute. Xác định khóa phân vùng và trường hợp cần thêm khóa sắp xếp để lưu nhiều mục có cùng khóa phân vùng.</li><li>Phác thảo cách đọc danh sách đơn hàng theo khách hàng bằng khóa đã chọn. Đối chiếu trường hợp một Region với bài toán cần đọc và ghi tại nhiều Region để hiểu vai trò của DynamoDB Global Tables.</li></ul> | 28/10/2026 | 28/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — NoSQL Database Services |
| Thứ Năm | **Phân tích demo RDS và DynamoDB**<ul><li>Theo dõi demo tạo cơ sở dữ liệu MySQL trên RDS, thêm dữ liệu vào các bảng và dùng JOIN để đọc thông tin có quan hệ.</li><li>Đối chiếu với demo tạo bảng DynamoDB và thêm item qua SDK. So sánh Query theo khóa với Scan đọc qua bảng, nêu cách khác biệt đó ảnh hưởng đến lượng dữ liệu được đọc. Ghi lại các tài nguyên phải kiểm tra nếu thực hiện lại demo.</li></ul> | 29/10/2026 | 29/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Databases Demonstration |
| Thứ Sáu | **Cache và cơ sở dữ liệu chuyên dụng**<ul><li>Vẽ luồng cache hit và cache miss giữa API, ElastiCache và RDS. Cân nhắc thời hạn cache và nguy cơ trả dữ liệu cũ sau một lần cập nhật.</li><li>Ghép DocumentDB với dữ liệu dạng tài liệu, Neptune với quan hệ dạng đồ thị, DAX với tăng tốc đọc DynamoDB và Managed Blockchain với tình huống dùng sổ cái phân tán. Liên hệ AWS Backup với yêu cầu khôi phục dữ liệu từ điểm sao lưu.</li></ul> | 30/10/2026 | 30/10/2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — In-Memory Caching Services<br>06 — Additional Database Services |

### Thành tựu Tuần 7

- Mẫu truy vấn, quan hệ giữa bản ghi và yêu cầu giao dịch là cơ sở chọn dịch vụ và khóa dữ liệu.
- Có thể phân biệt các bước JOIN trong RDS với Query và Scan trong DynamoDB qua demo của khóa học.
- Cache giảm lượt đọc trực tiếp vào cơ sở dữ liệu. Chính sách sao lưu và kiểm tra khôi phục giải quyết nhu cầu bảo toàn dữ liệu.
- **Áp dụng vào Tindy:** Nghiên cứu thiết kế cơ sở dữ liệu quan hệ RDS PostgreSQL 17 lưu trữ Profile, Project, Match data và lịch sử tin nhắn trò chuyện.

