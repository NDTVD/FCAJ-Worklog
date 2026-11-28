---
title: "Nhật ký Công việc Tuần 12"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

**Module 12** — Chiến lược Chuyển đổi Đám mây (7Rs), Hiện đại hóa Ứng dụng và Tự động hóa CI/CD

### Mục tiêu Tuần 12

- Nắm vững các giai đoạn chuyển đổi đám mây theo AWS Cloud Adoption Framework (CAF) và mô hình chiến lược 7Rs.
- Hiểu rõ các công cụ di chuyển dữ liệu online (AWS DataSync) và offline (AWS Snow Family) cho các quy mô dữ liệu khác nhau.
- Thiết lập quy trình tích hợp và phát hành liên tục (CI/CD) với GitHub Actions và AWS OIDC để tự động build và triển khai ứng dụng web.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Khung Chuyển đổi Đám mây AWS CAF & Các Giai đoạn Di chuyển**<ul><li>Khảo sát ba giai đoạn di chuyển chính: Đánh giá (Assess), Chuẩn bị lực lượng (Mobilize), và Di chuyển & Hiện đại hóa (Migrate and Modernize).</li><li>Đối chiếu 6 góc nhìn cốt lõi của AWS CAF: Kinh doanh (Business), Con người (People), Quản trị (Governance), Nền tảng (Platform), Bảo mật (Security) và Vận hành (Operations) để lập kế hoạch di chuyển toàn diện.</li></ul> | 30/11/2026 | 30/11/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Migration<br>02 — AWS Cloud Adoption Framework |
| Thứ Ba | **Chiến lược 7Rs & Hiện đại hóa Ứng dụng Web**<ul><li>Phân tích mô hình 7Rs: Rehost (Lift & Shift), Relocate (chuyển Hypervisor), Replatform (nâng cấp nền tảng nhẹ), Refactor (tái cấu trúc thành Cloud-Native), Repurchase (mua SaaS), Retain (giữ nguyên) và Retire (hủy bỏ).</li><li>Phân tích quá trình hiện đại hóa ứng dụng: chuyển đổi từ kiến trúc nguyên khối (Monolith) chạy trên máy chủ vật lý sang mô hình Container hóa (Replatform/Refactor) chạy trên ECS Fargate kết hợp Frontend tách biệt trên S3/CloudFront.</li></ul> | 01/12/2026 | 01/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Seven Migration Strategies<br>04 — Migration Services and Tools |
| Thứ Tư | **Di chuyển Cơ sở Dữ liệu với AWS Database Migration Service (DMS)**<ul><li>Khảo sát AWS DMS: công cụ hỗ trợ chuyển đổi cơ sở dữ liệu với thời gian gián đoạn tối thiểu (Downtime gần bằng 0).</li><li>Phân biệt di chuyển cùng hệ quản trị (Homogeneous: PostgreSQL sang RDS PostgreSQL) và khác hệ quản trị (Heterogeneous: Oracle sang PostgreSQL kết hợp AWS Schema Conversion Tool); tìm hiểu cơ chế đồng bộ thay đổi liên tục (Change Data Capture - CDC).</li></ul> | 02/12/2026 | 02/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Database Migrations |
| Thứ Năm | **Phương thức Chuyển Dữ liệu Online & Offline**<ul><li>So sánh các giải pháp truyền dữ liệu qua mạng (Online): AWS DataSync (truyền tệp tốc độ cao giữa NAS và S3/EFS), AWS Transfer Family (hỗ trợ SFTP/FTPS) và AWS Direct Connect (đường truyền mạng riêng vật lý).</li><li>Khảo sát các thiết bị vật lý chuyển dữ liệu ngoại tuyến (Offline): AWS Snowcone, Snowball Edge và Snowmobile cho các tập dữ liệu từ hàng chục Terabyte đến Exabyte khi băng thông mạng bị hạn chế.</li></ul> | 03/12/2026 | 03/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Transferring Data Online |
| Thứ Sáu | **Tự động Hóa Triển khai với GitHub Actions CI/CD & AWS OIDC**<ul><li>Nghiên cứu quy trình tự động hóa phát hành phần mềm: khi lập trình viên tạo Pull Request hoặc Push code lên nhánh `main`, pipeline CI/CD sẽ tự động kích hoạt.</li><li>Cấu hình pipeline GitHub Actions triển khai giao diện: chạy lệnh `npm install`, `npm run build` tạo thư mục `dist/`, sử dụng AWS OIDC để xác thực không cần mật khẩu, đồng bộ tệp lên S3 và tạo lệnh Invalidation làm mới bộ nhớ đệm CloudFront.</li></ul> | 04/12/2026 | 04/12/2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Transferring Data Offline |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Module 12 về chiến lược di chuyển lên đám mây (7Rs) và hiện đại hóa ứng dụng đã truyền cảm hứng rất lớn cho em về quy trình tự động hóa phát hành phần mềm hiện đại. Trước đây, mỗi lần cập nhật giao diện, em phải tự chạy build ở máy cá nhân rồi dùng phần mềm FTP hoặc giao diện Console để upload đè từng file lên máy chủ, quy trình này vừa mất thời gian vừa dễ xảy ra sai sót.

Trong dự án Tindy, em đã phối hợp thiết lập pipeline CI/CD hoàn chỉnh với GitHub Actions kết hợp xác thực bảo mật AWS OIDC. Giờ đây, mỗi khi em hoàn thành code giao diện mới và push lên nhánh main, toàn bộ quy trình từ cài đặt thư viện, build bundle React bằng Vite, đồng bộ thư mục dist/ lên S3 và tạo lệnh xóa cache CloudFront đều diễn ra hoàn toàn tự động chỉ trong vòng 90 giây.

### Thành tựu Tuần 12

- Khung AWS CAF và chiến lược 7Rs cung cấp lộ trình bài bản để chuyển đổi và hiện đại hóa các ứng dụng truyền thống lên đám mây.
- Tự động hóa CI/CD với xác thực AWS OIDC loại bỏ nguy cơ lộ lọt khóa bí mật và nâng cao tốc độ phát hành phần mềm.
- Áp dụng vào Tindy: Thiết lập pipeline GitHub Actions OIDC để tự động build React (npm run build), tải lên S3 và tạo invalidation CloudFront.
