---
title: "Nhật ký Công việc Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Module 8** — AI, Machine Learning và phân tích dữ liệu

### Mục tiêu Tuần 8

- Phân biệt huấn luyện, suy luận và các mức triển khai AI/ML trên AWS.
- Chọn công cụ Generative AI theo nhu cầu của ứng dụng và đội phát triển.
- Giải thích cách pipeline đưa dữ liệu từ nguồn đến lưu trữ, phân tích và huấn luyện mô hình.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **AI/ML và các lớp dịch vụ AWS**<ul><li>Theo dõi dữ liệu từ lúc chuẩn bị, huấn luyện mô hình đến khi suy luận. Dùng ví dụ gợi ý sản phẩm để phân biệt quy tắc viết tay với mô hình học từ dữ liệu.</li><li>Xếp lựa chọn AWS vào ba mức gồm dịch vụ AI dựng sẵn, Amazon SageMaker AI và framework chạy trên hạ tầng do đội ngũ tự quản lý. Giải thích sự đánh đổi giữa thời gian tích hợp và mức kiểm soát.</li></ul> | 02/11/2026 | 02/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to AI and Machine Learning<br>02 — AI-ML on AWS |
| Thứ Ba | **Chọn dịch vụ AI/ML theo tình huống**<ul><li>Đối chiếu Amazon Polly cho chuyển văn bản thành giọng nói và Amazon Comprehend cho phân tích ngôn ngữ. Trong mỗi trường hợp, xác định dữ liệu đầu vào và đầu ra mà backend sẽ dùng.</li><li>So sánh việc gọi một dịch vụ dựng sẵn với xây dựng mô hình riêng trên SageMaker AI. Xem dữ liệu huấn luyện, tiêu chí đánh giá và trách nhiệm vận hành nào sẽ phát sinh trước khi quyết định.</li></ul> | 03/11/2026 | 03/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS AI-ML Solutions |
| Thứ Tư | **Foundation model và Generative AI**<ul><li>Phân biệt foundation model với LLM và so sánh vai trò của Amazon Bedrock, SageMaker JumpStart, Amazon Q Business và Amazon Q Developer trong các tình huống của bài.</li><li>Liên hệ luồng bản nháp hồ sơ Tindy với Bedrock. Xác định đầu vào, cấu trúc kết quả và bước người dùng duyệt. Ôn cách RAG bổ sung ngữ cảnh bằng cách truy xuất dữ liệu liên quan để đưa vào yêu cầu.</li></ul> | 04/11/2026 | 04/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to Generative AI on AWS<br>05 — AWS Generative AI Solutions |
| Thứ Năm | **Từ nguồn dữ liệu đến báo cáo**<ul><li>Phân biệt data lake trên S3 với data warehouse và so sánh thứ tự xử lý của ETL, ELT và Zero-ETL theo ghi chú.</li><li>Vẽ quy trình thu nhận qua Kinesis Data Streams hoặc Data Firehose, lập danh mục và xử lý với Glue hoặc EMR, truy vấn qua Athena hoặc Redshift rồi trực quan hóa. Ghi rõ vấn đề chất lượng dữ liệu cần xử lý trước khi tạo báo cáo.</li></ul> | 05/11/2026 | 05/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Introduction to Data Analytics<br>07 — Data Pipelines on AWS |
| Thứ Sáu | **Kết hợp phân tích dữ liệu với ML**<ul><li>Lần theo ví dụ thay đổi dữ liệu DynamoDB đi qua Kinesis Data Streams và Data Firehose. Chú thích bước biến đổi bằng Lambda và nơi lưu trữ lâu dài trên S3.</li><li>Tách hai nhánh khai thác sau khi dữ liệu vào data lake. Athena dùng metadata từ Glue Data Catalog để truy vấn, còn SageMaker AI dùng dữ liệu phù hợp cho huấn luyện. Ghi cách kiểm tra tính nhất quán của dữ liệu cho hai nhánh.</li></ul> | 06/11/2026 | 06/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Data Analytics and AI-ML |

### Thành tựu Tuần 8

- Phân biệt dịch vụ AI dựng sẵn, nền tảng xây dựng mô hình và hạ tầng tự quản lý.
- Đầu ra Generative AI cần được kiểm tra theo tiêu chí của ứng dụng trước khi đưa vào hồ sơ hoặc quy trình nghiệp vụ.
- Một data lake có thể phục vụ phân tích và ML khi dữ liệu được xử lý, lập danh mục và kiểm tra chất lượng.
- **Áp dụng vào Tindy:** Tích hợp Amazon Bedrock để trích xuất kỹ năng từ CV; thiết kế giao diện AI Draft Review cho phép ứng viên xem lại và chỉnh sửa trước khi lưu.

