---
title: "Nhật ký Công việc Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Module 6** — Dịch vụ Lưu trữ Đám mây (Amazon S3, EBS, EFS) và Quản lý Tệp

### Mục tiêu Tuần 6

- Phân biệt ba mô hình lưu trữ cốt lõi: Object Storage (Amazon S3), Block Storage (Amazon EBS) và File Storage (Amazon EFS).
- Lựa chọn các phân hạng lưu trữ S3 (Storage Classes) và thiết lập chính sách vòng đời (S3 Lifecycle Rules) để tối ưu chi phí.
- Thực hành cấu hình lưu trữ web tĩnh, quản lý quyền truy cập S3 Bucket Policy và triển khai kỹ thuật tải tệp bằng S3 Presigned URLs.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Khảo sát Lưu trữ Đối tượng với Amazon S3**<ul><li>Tìm hiểu bản chất của Amazon S3: lưu trữ đối tượng (Object Storage) không giới hạn dung lượng với độ bền dữ liệu đạt 99.999999999% (11 số 9).</li><li>Nghiên cứu cấu trúc S3 Bucket: tên bucket độc nhất toàn cầu, cấu trúc Key phân cấp theo thư mục ảo, metadata đi kèm và cơ chế phiên bản hóa (S3 Versioning) chống ghi đè dữ liệu vô ý.</li></ul> | 19/10/2026 | 19/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Storage |
| Thứ Ba | **Phân hạng Lưu trữ S3 & Tự động hóa Vòng đời Tệp**<ul><li>So sánh các phân hạng lưu trữ: S3 Standard (truy cập thường xuyên), S3 Standard-IA (ít truy cập nhưng cần lấy ngay), S3 Glacier Instant Retrieval / Flexible Retrieval / Deep Archive (lưu trữ lưu trữ dài hạn giá siêu rẻ).</li><li>Tìm hiểu S3 Intelligent-Tiering: tự động di chuyển đối tượng giữa các tầng truy cập để tiết kiệm chi phí mà không phát sinh phí truy xuất dữ liệu; cấu hình S3 Lifecycle Policies tự động chuyển tệp CV cũ sau 90 ngày.</li></ul> | 20/10/2026 | 20/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — EC2 Instance Store and Amazon Elastic Block Store (Amazon EBS) |
| Thứ Tư | **Lưu trữ Khối Amazon EBS & Lưu trữ Tệp chia sẻ Amazon EFS**<ul><li>Nghiên cứu Amazon Elastic Block Store (EBS): ổ đĩa khối gắn trực tiếp vào máy chủ EC2, hỗ trợ Snapshot sao lưu tức thời và mã hóa EBS Encryption.</li><li>So sánh EBS với Amazon Elastic File System (EFS): hỗ trợ giao thức NFS cho phép hàng trăm máy chủ EC2 hoặc container ECS cùng đọc ghi tệp đồng thời.</li></ul> | 21/10/2026 | 21/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Amazon Elastic Block Store (Amazon EBS) Data Lifecycle |
| Thứ Năm | **Lưu trữ Web Tĩnh & Cơ chế Tải tệp Bằng S3 Presigned URLs**<ul><li>Khảo sát cách cấu hình S3 cho Static Website Hosting: thiết lập `index.html` làm trang chủ và cấu hình chuyển hướng cho Single Page Application (SPA).</li><li>Nghiên cứu kỹ thuật upload tối ưu: Client React gửi yêu cầu lấy Presigned URL có chữ ký bảo mật từ backend, sau đó trình duyệt upload trực tiếp tệp CV PDF lên S3 mà không làm nghẽn băng thông của máy chủ API.</li></ul> | 22/10/2026 | 22/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Amazon Simple Storage Service (Amazon S3) |
| Thứ Sáu | **Bảo mật S3 Bucket: Block Public Access & Origin Access Control**<ul><li>Tìm hiểu tính năng S3 Block Public Access để ngăn chặn nguy cơ rò rỉ dữ liệu do mở public bucket ra internet.</li><li>Nghiên cứu cấu hình S3 Bucket Policy kết hợp Origin Access Control (OAC): chỉ cho phép duy nhất dịch vụ CloudFront truy xuất các đối tượng tĩnh, ngăn người dùng truy cập trực tiếp qua link S3 gốc.</li></ul> | 23/10/2026 | 23/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon S3 Storage Classes and S3 Lifecycle<br>06 — Amazon S3 Demonstration |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần học về Storage giúp em nhận ra một giải pháp cực kỳ hiệu quả cho ứng dụng Tindy: cơ chế tải tệp lên qua S3 Presigned URL. Trước đây khi làm ứng dụng web, em thường gửi tệp binary qua API backend bằng `multipart/form-data`, điều này khiến máy chủ backend bị nghẽn RAM và mạng khi có nhiều người cùng upload CV một lúc.

Với S3 Presigned URL, phía Frontend của em chỉ cần gọi một API nhanh để nhận URL có chữ ký bảo mật với hạn dùng ngắn (5 phút), sau đó trình duyệt dùng lệnh `fetch()` với phương thức PUT gửi thẳng file PDF lên S3. Điều này vừa tăng tốc độ tải lên cho người dùng, vừa giải phóng máy chủ backend hoàn toàn.

### Thành tựu Tuần 6

- Amazon S3 là dịch vụ lưu trữ bền bỉ hàng đầu, hỗ trợ đa dạng phân hạng lưu trữ giúp tối ưu chi phí theo thời gian.
- Sử dụng Presigned URL là mẫu thiết kế chuẩn để tải tệp trực tiếp từ trình duyệt lên đám mây an toàn và hiệu năng cao.
- Áp dụng vào Tindy: Triển khai static build React lên S3; nghiên cứu quy trình lấy Presigned URL để người dùng tải CV PDF trực tiếp lên bucket.
