---
title: "Nhật ký Công việc Tuần 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Module 4** — AWS Regions, Mạng Biên (Edge Locations) và Tự động hóa Hạ tầng (CloudFormation)

### Mục tiêu Tuần 4

- Đánh giá các tiêu chí lựa chọn AWS Region tối ưu cho dự án (độ trễ người dùng, tính tuân thủ pháp lý, tính năng dịch vụ và bảng giá).
- Nắm vững vai trò của các điểm Edge Location và mạng phân phối nội dung Amazon CloudFront trong việc tối ưu hóa tốc độ tải trang web.
- Làm chủ khái niệm Infrastructure as Code (IaC) thông qua AWS CloudFormation: cấu trúc Template, Stack, Change Sets và cơ chế Rollback.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Phân bổ Hạ tầng Toàn cầu & Tiêu chí Chọn Region**<ul><li>Khảo sát 4 yếu tố then chốt khi chọn AWS Region: 1) Tuân thủ pháp lý và chủ quyền dữ liệu; 2) Khoảng cách địa lý tới nhóm người dùng mục tiêu; 3) Sự sẵn có của dịch vụ AWS cần dùng (ví dụ: Amazon Bedrock chỉ có ở một số Region); 4) Sự chênh lệch về chi phí giữa các vùng.</li><li>Phân tích vì sao Region US East (N. Virginia, us-east-1) thường là lựa chọn số một cho các dự án demo và startup công nghệ nhờ bảng giá tối ưu nhất.</li></ul> | 05/10/2026 | 05/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Going Global |
| Thứ Ba | **Mạng Biên Edge Locations & Amazon CloudFront**<ul><li>Tìm hiểu mạng lưới hơn 600 điểm hiện diện (PoP / Edge Locations) toàn cầu của AWS. Khảo sát nguyên lý hoạt động của CDN: lưu trữ đệm (caching) các tài nguyên tĩnh gần người dùng nhất.</li><li>Phân tích cơ chế giảm tải cho máy chủ gốc (Origin Shield) và cách CloudFront hỗ trợ SSL/TLS miễn phí với chứng chỉ AWS Certificate Manager (ACM).</li></ul> | 06/10/2026 | 06/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions |
| Thứ Tư | **Khái niệm Infrastructure as Code (IaC)**<ul><li>Tìm hiểu lợi ích của việc quản lý hạ tầng bằng mã: tính lặp lại (repeatability), kiểm soát phiên bản qua Git (version control), loại bỏ sai sót do cấu hình thủ công và khả năng nhân bản môi trường Dev/Staging/Prod tức thì.</li><li>So sánh việc tạo tài nguyên bằng giao diện Console với việc định nghĩa tài nguyên trong file cấu hình JSON/YAML.</li></ul> | 07/10/2026 | 07/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Diving Deeper into AWS Global Infrastructure |
| Thứ Năm | **Cấu trúc Template và Vòng đời Stack CloudFormation**<ul><li>Nghiên cứu cấu trúc một file CloudFormation Template chuẩn: AWSTemplateFormatVersion, Parameters (tham số đầu vào), Resources (tài nguyên bắt buộc), và Outputs (giá trị xuất ra để dùng cho stack khác).</li><li>Tìm hiểu tính năng Change Sets: xem trước các thay đổi tài nguyên trước khi áp dụng thực tế, cơ chế Drift Detection phát hiện sai khác cấu hình, và tính năng Rollback tự động khi có lỗi tạo tài nguyên.</li></ul> | 08/10/2026 | 08/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Infrastructure and Automation |
| Thứ Sáu | **Thực hành Thiết kế Bộ Template Triển khai**<ul><li>Phân tích phương pháp chia nhỏ hạ tầng thành nhiều stack độc lập theo trách nhiệm (Decoupled Stacks): Foundation, Network, Database, Integrations, Runtime và Edge.</li><li>Đánh giá cách sử dụng CloudFormation Outputs từ stack Network (VpcId, SubnetIds) làm Parameters đầu vào cho stack Database và Runtime, đảm bảo tính mô-đun hóa cao.</li></ul> | 09/10/2026 | 09/10/2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions<br>04 — Infrastructure and Automation |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Module 4 giúp em hiểu được khái niệm Infrastructure as Code (IaC) thông qua AWS CloudFormation. Nhìn cách một hệ thống phức tạp gồm hàng chục tài nguyên (VPC, Subnets, ALB, ECS, S3) được định nghĩa mạch lạc trong các file YAML giúp em thấy rõ sự chuyên nghiệp so với việc bấm tay thủ công trên AWS Console.

Đối với người làm giao diện web, kiến thức về Edge Location và CloudFront trong tuần này đặc biệt hữu ích. Em hiểu được cơ chế phân phối tĩnh: thay vì người dùng phải tải từng file bundle .js, .css từ máy chủ gốc ở Virginia với độ trễ cao, CloudFront sẽ lưu đệm các file tĩnh này tại các điểm Edge gần người dùng nhất tại Việt Nam, giúp tốc độ mở trang Tindy nhanh gấp nhiều lần.

### Thành tựu Tuần 4

- Infrastructure as Code (CloudFormation) là tiêu chuẩn bắt buộc trong kỹ thuật phần mềm hiện đại để tự động hóa việc dựng và dọn dẹp môi trường.
- Amazon CloudFront kết hợp Edge Location giúp giảm tải tối đa cho máy chủ backend và tăng tốc độ tải trang web vượt bậc.
- Áp dụng vào Tindy: Lựa chọn Region us-east-1 cho toàn bộ hệ thống; nghiên cứu cách CloudFront phân phối static bundle React tới người dùng với độ trễ thấp.
