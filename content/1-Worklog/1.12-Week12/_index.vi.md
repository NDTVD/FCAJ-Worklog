---
title: "Nhật ký Công việc Tuần 12"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

**Module 12** — Chiến lược migration và chuyển dữ liệu lên AWS

### Mục tiêu Tuần 12

- Nêu các giai đoạn migration và cách AWS CAF hỗ trợ chuẩn bị tổ chức.
- Chọn chiến lược trong mô hình 7R và nhận diện công cụ phù hợp cho ứng dụng hoặc cơ sở dữ liệu.
- So sánh phương án chuyển dữ liệu online và offline theo dung lượng, thời gian và băng thông.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Các giai đoạn migration và AWS CAF**<ul><li>Lập danh sách công việc trong ba giai đoạn Assess, Mobilize, Migrate and Modernize. Dùng ví dụ backend .NET để nhận diện phụ thuộc như PostgreSQL, lưu trữ tệp và xác thực trước khi di chuyển.</li><li>Ghép các việc chuẩn bị với sáu góc nhìn của AWS CAF gồm Business, People, Governance, Platform, Security và Operations. Xác định ai chịu trách nhiệm đánh giá, chuẩn bị và vận hành sau chuyển đổi.</li></ul> | 30/11/2026 | 30/11/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Migration<br>02 — AWS Cloud Adoption Framework |
| Thứ Ba | **Bảy chiến lược và công cụ migration**<ul><li>So sánh rehost, relocate, replatform, refactor, repurchase, retain và retire. Dùng ví dụ chuyển PostgreSQL tự vận hành sang RDS để giải thích lựa chọn replatform.</li><li>Đọc vai trò của kiểm kê phụ thuộc, ước tính chi phí, chuyển máy chủ và theo dõi tiến độ. Đối chiếu AWS Application Migration Service với các công cụ lập kế hoạch và ghi nhận các công cụ được giới thiệu trong transcript theo bối cảnh của bài.</li></ul> | 01/12/2026 | 01/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Seven Migration Strategies<br>04 — Migration Services and Tools |
| Thứ Tư | **Di chuyển cơ sở dữ liệu bằng AWS DMS**<ul><li>Phân biệt migration cùng hệ quản trị và khác hệ quản trị. Xác định trường hợp phải chuyển đổi schema trước khi di chuyển dữ liệu và vai trò của AWS DMS cùng công cụ chuyển đổi schema.</li><li>Lập kế hoạch mẫu cho PostgreSQL gồm chép dữ liệu ban đầu, theo dõi thay đổi bằng CDC khi phù hợp, kiểm tra số bản ghi và xác nhận giao dịch trước cutover. Ghi điều kiện dừng hoặc quay lại nguồn nếu đối soát thất bại.</li></ul> | 02/12/2026 | 02/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Database Migrations |
| Thứ Năm | **Chuyển dữ liệu qua mạng**<ul><li>So sánh DataSync để chuyển tập dữ liệu giữa các hệ thống lưu trữ, Transfer Family để nhận tệp qua giao thức được hỗ trợ và Direct Connect để cung cấp kết nối chuyên dụng.</li><li>Ước tính thời gian sao chép thư mục media từ dung lượng và thông lượng thực tế. Phân biệt công việc chuyển tệp một lần với kết nối lâu dài và xác định cách kiểm tra tệp ở đích.</li></ul> | 03/12/2026 | 03/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Transferring Data Online |
| Thứ Sáu | **Chuyển dữ liệu offline và đánh giá đánh đổi**<ul><li>Đọc ví dụ Snowball Edge trong tài liệu để hiểu quá trình chép dữ liệu vào thiết bị, vận chuyển và nhập vào AWS. Liên hệ xử lý tại edge với môi trường thiếu kết nối ổn định.</li><li>So sánh tổng thời gian sao chép, vận chuyển và nhập dữ liệu với phương án online. Khi lập phương án mẫu, ghi rõ cần kiểm tra khả năng sử dụng dịch vụ và chọn cách xác minh tính toàn vẹn sau chuyển.</li></ul> | 04/12/2026 | 04/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Transferring Data Offline |

### Thành tựu Tuần 12

- Kiểm kê phụ thuộc và các góc nhìn AWS CAF giúp xác định công việc cần hoàn thành trước cutover.
- 7R phân biệt mức thay đổi của ứng dụng. Với dữ liệu, chuyển đổi schema, tải ban đầu và áp dụng thay đổi là các việc cần lập kế hoạch riêng.
- Ước tính thời gian truyền cần xét thông lượng thực tế, thời gian gián đoạn và cách đối soát dữ liệu sau chuyển.
- **Áp dụng vào Tindy:** Thiết lập quy trình CI/CD với GitHub Actions OIDC để tự động build React (npm run build), tải lên S3 và tạo invalidation CloudFront.

