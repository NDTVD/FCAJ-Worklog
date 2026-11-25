---
title: "Nhật ký Công việc Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

**Module 1** — Nền tảng AWS Cloud và hạ tầng

### Mục tiêu Tuần 1

- Giải thích mô hình client–server, cách cấp phát tài nguyên theo nhu cầu và cách trả phí theo mức sử dụng.
- Phân biệt Region, Availability Zone và trung tâm dữ liệu để chọn vị trí triển khai phù hợp.
- Áp dụng mô hình trách nhiệm chia sẻ với Amazon EC2, Amazon RDS và Amazon S3.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Điện toán đám mây và mô hình client–server**<ul><li>Tìm hiểu vai trò của client và server trong một yêu cầu, mô hình cấp phát theo nhu cầu và cách trả phí theo mức sử dụng.</li><li>Vẽ luồng từ trình duyệt gửi yêu cầu đến máy chủ rồi nhận phản hồi. Dùng ví dụ cửa hàng trực tuyến để xác định dữ liệu nào do client gửi và công việc nào do server xử lý. Ghi lại sự khác nhau giữa mua sẵn máy chủ và cấp phát tài nguyên theo nhu cầu.</li></ul> | 14/09/2026 | 14/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01–02 — Welcome to AWS Cloud Practitioner Essentials<br>What is Cloud Computing |
| Thứ Ba | **Sáu lợi ích của AWS Cloud**<ul><li>Hệ thống hóa sáu lợi ích của AWS Cloud qua ví dụ cửa hàng trực tuyến.</li><li>Lập bảng sáu lợi ích của AWS Cloud, mỗi lợi ích đi kèm một tình huống. Chẳng hạn, mô tả cách cửa hàng đáp ứng thêm lượt truy cập trong đợt khuyến mãi và giảm công suất khi nhu cầu trở lại bình thường.</li></ul> | 15/09/2026 | 15/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Benefits of the AWS Cloud |
| Thứ Tư | **Hạ tầng toàn cầu của AWS**<ul><li>So sánh Region, Availability Zone và data center. Ôn vai trò của Multi-AZ và Multi-Region.</li><li>Vẽ quan hệ giữa Region, Availability Zone và data center. Dùng tình huống mất một AZ để giải thích ảnh hưởng đến ứng dụng đặt trong một AZ và ứng dụng có tài nguyên ở nhiều AZ. Ghi thêm khi nào cần xem xét một Region thứ hai.</li></ul> | 16/09/2026 | 16/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to AWS Global Infrastructure |
| Thứ Năm | **Mô hình trách nhiệm chia sẻ**<ul><li>Phân tích trách nhiệm bảo mật khi dùng Amazon EC2, Amazon RDS và Amazon S3.</li><li>Chia trách nhiệm thành hai cột AWS và khách hàng, rồi điền ví dụ cho EC2, RDS và S3. Theo dõi riêng trách nhiệm quản lý hệ điều hành, cấu hình quyền truy cập và dữ liệu để thấy sự khác nhau giữa các loại dịch vụ.</li></ul> | 17/09/2026 | 17/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — The AWS Shared Responsibility Model |
| Thứ Sáu | **Tình huống thương mại điện tử**<ul><li>Liên hệ vị trí triển khai, độ trễ và tính sẵn sàng với ví dụ thương mại điện tử.</li><li>Phác thảo cách triển khai cửa hàng phục vụ người dùng ở hai khu vực. Giải thích lựa chọn Region dựa trên độ trễ, sau đó xác định phần nào của kiến trúc cần dự phòng qua nhiều AZ. Tóm tắt trách nhiệm bảo mật còn lại của đội ứng dụng.</li></ul> | 18/09/2026 | 18/09/2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Applying Cloud Concepts to Real Life Use Cases |

### Thành tựu Tuần 1

- Trả phí theo mức sử dụng và điều chỉnh tài nguyên theo nhu cầu giúp giảm việc phải dự đoán công suất trước.
- Multi-AZ giúp ứng dụng chịu được sự cố ở một AZ. Trách nhiệm bảo mật của khách hàng thay đổi theo dịch vụ sử dụng.
- **Áp dụng vào Tindy:** Phân tích luồng Client–Server giữa React Frontend (Vite) và API ASP.NET Core; tìm hiểu cơ chế trả phí theo nhu cầu thực tế để kiểm soát chi phí cho các tài nguyên demo.

