---
title: "Nhật ký Công việc Tuần 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Module 4** — AWS Region và tự động hóa hạ tầng

### Mục tiêu Tuần 4

- Phân biệt vai trò của Region, Availability Zone và Edge Location khi phục vụ người dùng toàn cầu.
- Đánh giá Region theo vị trí người dùng, yêu cầu tuân thủ, tính khả dụng của dịch vụ và chi phí.
- Giải thích cách AWS CloudFormation mô tả, triển khai và kiểm tra thay đổi hạ tầng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Triển khai cho người dùng toàn cầu**<ul><li>Ôn vai trò của Region và Edge Location trong việc phục vụ người dùng toàn cầu.</li><li>Phân biệt vị trí triển khai backend với vị trí phân phối nội dung gần người dùng. Vẽ hành trình một yêu cầu từ trình duyệt đến nội dung ở edge và đến ứng dụng ở Region, rồi ghi cách từng vị trí ảnh hưởng đến độ trễ.</li></ul> | 05/10/2026 | 05/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Going Global |
| Thứ Ba | **Tiêu chí chọn AWS Region**<ul><li>Đánh giá lựa chọn Region theo yêu cầu tuân thủ, khoảng cách tới người dùng, tính khả dụng của dịch vụ và chi phí.</li><li>Tạo ma trận lựa chọn Region cho ứng dụng phục vụ hai nhóm người dùng. Đánh dấu yêu cầu bắt buộc về nơi lưu trữ dữ liệu và tính khả dụng của dịch vụ trước khi cân nhắc độ trễ và chi phí giữa các lựa chọn còn lại.</li></ul> | 06/10/2026 | 06/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions |
| Thứ Tư | **Bố trí tài nguyên trong hạ tầng AWS**<ul><li>Ôn cấu trúc Region, Availability Zone và Edge Location từ góc nhìn triển khai ứng dụng.</li><li>Dùng ví dụ ứng dụng đặt trong hai AZ để phân biệt quyết định chọn Region với quyết định bố trí tài nguyên trong Region đó. Giải thích tình huống nào cần dự phòng theo AZ và ghi lý do có thể phải phục vụ từ nhiều Region.</li></ul> | 07/10/2026 | 07/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Diving Deeper into AWS Global Infrastructure |
| Thứ Năm | **Template, stack và quản lý thay đổi**<ul><li>Tìm hiểu CloudFormation template và stack. Ôn công dụng của change sets, drift detection và StackSets.</li><li>Chú thích một template theo tham số, tài nguyên và đầu ra. Sau đó nối mỗi thao tác với công cụ phù hợp: xem trước thay đổi với change set, phát hiện sai khác với drift detection và dùng StackSets khi cần quản lý triển khai trên nhiều tài khoản hoặc Region.</li></ul> | 08/10/2026 | 08/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Infrastructure and Automation |
| Thứ Sáu | **Tình huống chọn Region và chuẩn bị cấu hình**<ul><li>Chọn Region cho một ứng dụng mẫu, giải thích lựa chọn theo tiêu chí đã học và phác thảo các tham số cần đưa vào template CloudFormation.</li><li>Đưa quyết định chọn Region vào một cấu hình triển khai có thể lặp lại. Phân biệt thông số cố định trong template với thông số cần truyền khi tạo stack. Dùng danh sách tham số và đầu ra dự kiến làm bước chuẩn bị cho bài lab tuần sau.</li></ul> | 09/10/2026 | 09/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions<br>04 — Infrastructure and Automation |

### Thành tựu Tuần 4

- Lựa chọn Region cần cân bằng độ trễ với yêu cầu về vị trí lưu trữ dữ liệu, tính năng dịch vụ và chi phí.
- CloudFormation dùng template để mô tả hạ tầng và stack để quản lý tập tài nguyên được triển khai từ template.
- **Áp dụng vào Tindy:** Lựa chọn Region us-east-1 cho toàn bộ hệ thống; nghiên cứu cách CloudFront phân phối static bundle React tới người dùng với độ trễ thấp.

