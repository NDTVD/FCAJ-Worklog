---
title: "Nhật ký Công việc Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Module 11** — Định giá, hỗ trợ và tối ưu chi phí AWS

### Mục tiêu Tuần 11

- Nhận diện các yếu tố tính phí khi chạy ứng dụng và giải thích khi nào nên cân nhắc cam kết sử dụng.
- Đọc chi phí, phân bổ chi phí theo nhãn và thiết kế cảnh báo ngân sách.
- So sánh nhu cầu hỗ trợ kỹ thuật và đánh giá phương án tối ưu bằng số liệu sử dụng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Cơ chế định giá và nguồn chi phí**<ul><li>Phân biệt trả theo mức sử dụng, tiết kiệm khi cam kết và đơn giá theo bậc. Liệt kê ba nhóm chi phí cơ bản là compute, storage và truyền dữ liệu ra ngoài.</li><li>Đối chiếu một lần chạy demo Tindy với kịch bản chạy liên tục. Ghi riêng số giờ chạy Fargate và RDS, thời gian giữ ALB, dung lượng S3, log và snapshot để thấy khoản nào tiếp tục phát sinh giữa các buổi demo.</li></ul> | 23/11/2026 | 23/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Pricing and Support<br>02 — AWS Pricing Concepts |
| Thứ Ba | **Billing Dashboard, AWS Budgets và Cost Explorer**<ul><li>Phân biệt nơi xem chi phí hiện tại, công cụ phân tích xu hướng và nơi thiết lập ngưỡng cảnh báo. Đọc ví dụ chi phí thực tế và chi phí dự báo trong AWS Budgets.</li><li>Phác thảo nhóm chi phí theo dịch vụ, tài khoản và tag dự án. Xác định tag cần kích hoạt để phân bổ chi phí, rồi liên hệ thanh toán hợp nhất với việc đọc hóa đơn của nhiều tài khoản.</li></ul> | 24/11/2026 | 24/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Pricing and Billing Services |
| Thứ Tư | **Đánh giá nhu cầu AWS Support**<ul><li>So sánh hỗ trợ về tài khoản và thanh toán với hỗ trợ kỹ thuật cho workload đang vận hành. Dựa trên tình huống trong bài để xác định mức ảnh hưởng và nhu cầu phản hồi.</li><li>Soạn nội dung mẫu cho một yêu cầu hỗ trợ gồm triệu chứng, thời điểm, Region, phạm vi ảnh hưởng và kiểm tra đã thực hiện. Phân biệt thời gian phản hồi ban đầu với thời gian giải quyết vấn đề.</li></ul> | 25/11/2026 | 25/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Support Plans |
| Thứ Năm | **AWS Marketplace và AWS Partner Network**<ul><li>Phân biệt tìm sản phẩm hoặc dịch vụ qua AWS Marketplace với tìm đối tác có chuyên môn triển khai, tích hợp hoặc migration qua AWS Partner Network.</li><li>Đánh giá một công cụ bên thứ ba theo mô hình tính phí, điều khoản, quyền truy cập và công việc vận hành. Tách khoản phí của nhà cung cấp khỏi chi phí tài nguyên AWS phát sinh khi chạy công cụ.</li></ul> | 26/11/2026 | 26/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — AWS Marketplace and AWS Partners |
| Thứ Sáu | **Tối ưu chi phí dựa trên mức sử dụng**<ul><li>Đọc ví dụ rightsizing compute, kiểm tra mức sử dụng RDS và chọn lifecycle cho dữ liệu S3. Đánh giá đường truyền và trường hợp có thể dùng S3 Gateway Endpoint thay cho đường qua NAT trong kiến trúc phù hợp.</li><li>Lập quy trình đo chi phí hiện tại, chọn một thay đổi, theo dõi tác động rồi kiểm tra hiệu suất sau thay đổi. Ưu tiên xử lý tài nguyên demo không cần chạy liên tục và liệt kê dữ liệu phải giữ để phục hồi.</li></ul> | 27/11/2026 | 27/11/2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Cost Optimization |

### Thành tựu Tuần 11

- Chi phí ứng dụng phụ thuộc cả thời lượng chạy và tài nguyên lưu lại giữa các lần sử dụng.
- Billing Dashboard, Budgets và Cost Explorer lần lượt hỗ trợ xem chi phí, nhận cảnh báo và phân tích xu hướng.
- Một đề xuất tối ưu cần có số liệu trước và sau, kỳ vọng vận hành và phương án bảo toàn dữ liệu.
- **Áp dụng vào Tindy:** Thực hành ước tính chi phí qua AWS Pricing Calculator (~.32/tháng) và áp dụng chiến lược chạy demo theo lịch để giữ chi phí thực tế dưới .

