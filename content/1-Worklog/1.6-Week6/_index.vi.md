---
title: "Nhật ký Công việc Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Module 6** — Lưu trữ AWS, EBS và S3

### Mục tiêu Tuần 6

- Chọn lưu trữ theo block, object hoặc file dựa trên cách ứng dụng truy cập dữ liệu.
- Phân biệt EC2 Instance Store với Amazon EBS, đồng thời giải thích vai trò của snapshot và chính sách lưu giữ.
- Hiểu cấu trúc Amazon S3 và chọn storage class, quy tắc chuyển lớp hoặc hết hạn phù hợp.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Block, object và file storage**<ul><li>So sánh block, object và file storage qua các ví dụ với Amazon EBS, Amazon S3 và Amazon EFS.</li><li>So sánh ba cách ứng dụng truy cập dữ liệu: ổ đĩa theo block, đối tượng theo key và tệp qua hệ thống file dùng chung. Dùng ví dụ database trên EC2, ảnh do người dùng tải lên và thư mục dùng chung để chọn EBS, S3 hoặc EFS.</li></ul> | 19/10/2026 | 19/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Storage |
| Thứ Ba | **EC2 Instance Store và Amazon EBS**<ul><li>Đối chiếu EC2 Instance Store và Amazon EBS theo khả năng giữ dữ liệu khi instance thay đổi trạng thái.</li><li>Lập bảng trạng thái reboot, stop và terminate cho instance store và EBS. Ghi tình huống nào phù hợp cho tệp tạm, tình huống nào cần volume lưu dữ liệu lâu hơn và thiết lập nào ảnh hưởng đến việc giữ EBS khi chấm dứt instance.</li></ul> | 20/10/2026 | 20/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — EC2 Instance Store and Amazon Elastic Block Store (Amazon EBS) |
| Thứ Tư | **Snapshot và vòng đời EBS**<ul><li>Tìm hiểu snapshot tăng dần, khôi phục volume từ snapshot và tự động hóa lịch sao lưu bằng Amazon Data Lifecycle Manager.</li><li>Vẽ một chuỗi snapshot để thể hiện phần dữ liệu thay đổi giữa các lần sao lưu. Giải thích cách tạo volume mới từ một điểm khôi phục và phác thảo chính sách DLM với lịch tạo snapshot cùng thời hạn lưu giữ.</li></ul> | 21/10/2026 | 21/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Amazon Elastic Block Store (Amazon EBS) Data Lifecycle |
| Thứ Năm | **Bucket, object và metadata của Amazon S3**<ul><li>Tìm hiểu bucket, object, key và metadata. Phân biệt độ bền dữ liệu với tính khả dụng.</li><li>Mô tả cách bucket chứa object, object được nhận diện theo key và metadata mô tả dữ liệu. Dùng ví dụ tệp hồ sơ để phân biệt quyền đọc object, khả năng truy cập dịch vụ tại một thời điểm và khả năng dữ liệu được lưu bền vững.</li></ul> | 22/10/2026 | 22/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Amazon Simple Storage Service (Amazon S3) |
| Thứ Sáu | **Storage class, S3 Lifecycle và demo**<ul><li>So sánh các storage class theo tần suất truy cập, thời gian truy xuất và chi phí. Đọc ví dụ chuyển lớp và hết hạn đối tượng trong S3 Lifecycle. Phân tích demo tạo bucket, tải object lên, xem metadata và tìm hiểu bucket policy và S3 Versioning.</li><li>Chọn lớp lưu trữ cho ảnh thường xem, dữ liệu ít truy cập và bản lưu dài hạn. Viết một ví dụ S3 Lifecycle có mốc chuyển lớp và hết hạn. Đối chiếu với demo trên Console để xác định thông tin bucket, object và lịch sử phiên bản cần kiểm tra.</li></ul> | 23/10/2026 | 23/10/2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon S3 Storage Classes and S3 Lifecycle<br>06 — Amazon S3 Demonstration |

### Thành tựu Tuần 6

- Instance Store phù hợp với dữ liệu tạm, EBS duy trì dữ liệu theo vòng đời của volume và snapshot cung cấp điểm khôi phục.
- Chọn storage class theo cách sử dụng dữ liệu. S3 Lifecycle tự động chuyển lớp lưu trữ hoặc đặt thời điểm hết hạn cho object.
- **Áp dụng vào Tindy:** Cấu hình Amazon S3 lưu trữ bản build tĩnh của Frontend (qua OAC) và S3 Media Bucket lưu trữ CV PDF người dùng tải lên.

