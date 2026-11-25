---
title: "Nhật ký Công việc Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Module 5** — Amazon VPC, bảo mật và mạng toàn cầu

### Mục tiêu Tuần 5

- Lần theo đường đi của lưu lượng qua VPC, subnet và route table.
- Phân biệt security group với network ACL và chọn phương án kết nối theo từng tình huống.
- Giải thích vai trò của Route 53, CloudFront và Global Accelerator trong kiến trúc mạng toàn cầu.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **VPC và ranh giới mạng**<ul><li>Tìm hiểu nhu cầu kết nối tài nguyên AWS, mạng chi nhánh và người dùng từ xa. Phân tích phạm vi của VPC và vai trò của Internet Gateway và Virtual Private Gateway.</li><li>Vẽ VPC như ranh giới mạng của ứng dụng, sau đó thêm đường kết nối internet, mạng chi nhánh và người dùng làm việc từ xa. Giải thích trường hợp nào đi qua internet gateway và trường hợp nào cần xem xét virtual private gateway cho kết nối riêng.</li></ul> | 12/10/2026 | 12/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Networking<br>02 — Organizing AWS Cloud Resources |
| Thứ Ba | **Kết nối người dùng, mạng và dịch vụ**<ul><li>Đối chiếu AWS Client VPN, AWS Site-to-Site VPN, AWS Direct Connect và AWS PrivateLink theo tình huống sử dụng.</li><li>Dùng các kịch bản nhân viên làm việc từ xa, kết nối văn phòng, nhu cầu đường truyền chuyên dụng và truy cập riêng một dịch vụ. Với mỗi kịch bản, chọn Client VPN, Site-to-Site VPN, Direct Connect hoặc PrivateLink và giải thích phạm vi kết nối cần thiết.</li></ul> | 13/10/2026 | 13/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — More Ways to Connect to the AWS Cloud |
| Thứ Tư | **Subnet, định tuyến và kiểm soát lưu lượng**<ul><li>So sánh public/private subnet, Security Group có trạng thái và Network ACL phi trạng thái. Phân tích demo VPC với public/private subnets trên hai AZ, Internet Gateway và route table.</li><li>Lần theo yêu cầu đến máy chủ trong sơ đồ VPC có subnet public và private trải trên hai AZ. Đọc tuyến đường trong route table rồi kiểm tra hai lớp lọc: security group theo dõi trạng thái kết nối, còn network ACL cần xét quy tắc ở cả chiều đi và chiều về.</li></ul> | 14/10/2026 | 14/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Subnets, Security Groups, and Network Access Control Lists<br>05 — Amazon VPC Demo |
| Thứ Năm | **DNS, phân phối nội dung và tăng tốc mạng**<ul><li>Phân biệt DNS trong Route 53, phân phối nội dung qua CloudFront và tăng tốc lưu lượng qua Global Accelerator.</li><li>Dùng ví dụ ứng dụng có tên miền riêng và nội dung tĩnh để phân biệt điểm giải quyết tên miền với điểm phục vụ nội dung. Chú thích vai trò của Route 53, CloudFront và Global Accelerator trên sơ đồ thay vì gộp cả ba vào một lớp xử lý.</li></ul> | 15/10/2026 | 15/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Global Networking |
| Thứ Sáu | **Kiến trúc dự phòng và phân phối toàn cầu**<ul><li>Đọc ví dụ kiến trúc dự phòng kết nối Direct Connect và phân phối nội dung cho người dùng ở nhiều Region.</li><li>Đọc hai tình huống, một về dự phòng đường kết nối Direct Connect và một về phân phối nội dung ở nhiều Region. So sánh thành phần cần dự phòng ở mỗi tình huống và viết một sơ đồ ngắn cho biết điều gì xảy ra khi một đường kết nối hoặc một đích không khả dụng.</li></ul> | 16/10/2026 | 16/10/2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Global Architectures |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần 5 là một trong những tuần học quan trọng nhất đối với em vì liên quan trực tiếp đến việc định tuyến mạng và bảo mật kết nối. Em đã hiểu rõ cấu trúc của Amazon VPC: sự phân chia giữa Public Subnet (dành cho các dịch vụ cần giao tiếp ra ngoài) và Private Subnet (nơi bảo vệ cơ sở dữ liệu PostgreSQL).

Đặc biệt, em tìm hiểu sâu về cách CloudFront VPC Origin kết hợp với Internal ALB. Nhờ mô hình này, API backend của nhóm hoàn toàn không cần mở public ra Internet mà vẫn nhận được request an toàn từ CloudFront. Đây cũng là tuần em nghiên cứu kỹ về lỗi CORS (Cross-Origin Resource Sharing) để chuẩn bị cho việc cấu hình Program.cs ở Backend, bảo đảm trình duyệt không chặn các request gọi API và WebSocket.

### Thành tựu Tuần 5

- Client VPN phục vụ người dùng từ xa, Site-to-Site VPN kết nối các mạng, Direct Connect cung cấp kết nối chuyên dụng và PrivateLink hỗ trợ truy cập riêng tới dịch vụ.
- Route table quyết định đường đi của lưu lượng trong VPC. Ở lớp phục vụ người dùng toàn cầu, Route 53 xử lý DNS, CloudFront phân phối nội dung và Global Accelerator tối ưu đường đi của lưu lượng.
- **Áp dụng vào Tindy:** Hiểu cách phân tách mạng VPC với Private Subnet cho Database và cấu hình CloudFront VPC Origin kết nối an toàn tới Internal ALB.


