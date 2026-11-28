---
title: "Nhật ký Công việc Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Module 8** — Trí tuệ Nhân tạo (AI/ML), Amazon Bedrock và Xử lý CV Thông minh

### Mục tiêu Tuần 8

- Nắm bắt tổng quan về AI/ML trên AWS và phân biệt Trí tuệ Nhân tạo Tạo sinh (Generative AI) với AI truyền thống.
- Hiểu kiến trúc dịch vụ không máy chủ của Amazon Bedrock và các mô hình nền tảng (Foundation Models) như Anthropic Claude.
- Làm chủ kỹ thuật Prompt Engineering để trích xuất dữ liệu có cấu trúc từ hồ sơ CV PDF và hiển thị trực quan trên giao diện người dùng.

### Các nhiệm vụ trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| Thứ Hai | **Tổng quan Dịch vụ AI/ML & Xu hướng Generative AI trên AWS**<ul><li>Khảo sát các tầng AI/ML trên AWS: Tầng ứng dụng (Rekognition, Textract, Polly), Tầng nền tảng (Amazon SageMaker) và Tầng Generative AI tiên tiến (Amazon Bedrock).</li><li>Phân tích tiềm năng ứng dụng Generative AI trong việc giải quyết bài toán ghép nối dự án sinh viên: tự động đọc hiểu hồ sơ năng lực và gợi ý vị trí tuyển dụng phù hợp nhất.</li></ul> | 02/11/2026 | 02/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to AI and Machine Learning<br>02 — AI-ML on AWS |
| Thứ Ba | **Khám phá Amazon Bedrock & Các Mô hình Nền tảng (Foundation Models)**<ul><li>Tìm hiểu Amazon Bedrock: dịch vụ được quản lý toàn diện (Fully Managed) cung cấp quyền truy cập các Foundation Models (FM) hàng đầu thông qua một API thống nhất duy nhất.</li><li>So sánh các dòng mô hình của Anthropic (Claude 3 Haiku nhanh nhẹ, Claude 3 Sonnet cân bằng giữa tốc độ và trí tuệ, Claude 3 Opus chuyên sâu); tìm hiểu các siêu tham số (Hyperparameters): Temperature, TopP, Max Tokens.</li></ul> | 03/11/2026 | 03/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS AI-ML Solutions |
| Thứ Tư | **Kỹ thuật Prompt Engineering & Trích xuất JSON từ PDF**<ul><li>Nghiên cứu nghệ thuật Prompt Engineering: thiết lập vai trò hệ thống (System Role), cung cấp ngữ cảnh rõ ràng và áp dụng kỹ thuật Few-shot Prompting để định dạng kết quả.</li><li>Xây dựng prompt chuyên dụng yêu cầu model phân tích nội dung văn bản CV PDF và trả về đúng định dạng JSON chuẩn (gồm: Họ tên, Kỹ năng kỹ thuật, Năm kinh nghiệm, Định hướng nghề nghiệp) mà không kèm theo lời giải thích dư thừa.</li></ul> | 04/11/2026 | 04/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to Generative AI on AWS<br>05 — AWS Generative AI Solutions |
| Thứ Năm | **Thiết kế Giao diện AI Studio & Trải nghiệm Phản hồi Thời gian thực**<ul><li>Xây dựng màn hình AI Studio trên React: cho phép người dùng chọn tệp CV PDF, hiển thị tiến trình quét (Scanning Animation) và hiển thị kết quả trích xuất dạng thẻ sinh động.</li><li>Thiết kế cơ chế xác nhận người dùng (Human-in-the-loop): cho phép sinh viên chỉnh sửa hoặc chọn lọc các kỹ năng do AI gợi ý trước khi lưu chính thức vào hồ sơ cá nhân.</li></ul> | 05/11/2026 | 05/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Introduction to Data Analytics<br>07 — Data Pipelines on AWS |
| Thứ Sáu | **Tối ưu Hóa Chi phí Gọi Model & Nguyên tắc Bảo mật AI (Responsible AI)**<ul><li>Phân tích cơ chế tính phí của Bedrock theo số lượng Token đầu vào (Input Tokens) và Token đầu ra (Output Tokens). Tìm hiểu cách cắt tỉa văn bản trước khi gửi để tiết kiệm chi phí.</li><li>Nghiên cứu nguyên tắc Responsible AI: đảm bảo dữ liệu CV cá nhân của sinh viên được bảo vệ an toàn, không bị sử dụng để huấn luyện lại các mô hình công cộng của bên thứ ba.</li></ul> | 06/11/2026 | 06/11/2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Data Analytics and AI-ML |

### Ghi chép & Góc nhìn cá nhân của Cao Thành Nhân

Tuần học về Amazon Bedrock và Generative AI là một trong những trải nghiệm thú vị nhất đối với em. Với giao diện AI Studio trong Tindy, việc tạo ra một trải nghiệm mượt mà cho tính năng quét CV bằng AI đòi hỏi sự kết hợp chặt chẽ giữa Frontend và Cloud.

Người dùng thường cảm thấy sốt ruột nếu màn hình đứng yên trong lúc AI đang xử lý (thường mất từ 3-6 giây). Em đã thiết kế các hiệu ứng hoạt họa quét tài liệu (Scanning Animation) và thanh tiến trình từng bước, giúp người dùng hiểu rõ hệ thống đang đọc tệp, trích xuất kỹ năng và phân tích hồ sơ. Đặc biệt, việc hiển thị các kỹ năng AI gợi ý dưới dạng các ô thẻ (Chips) có thể bấm chọn/xóa giúp người dùng nắm toàn quyền quyết định dữ liệu của mình.

### Thành tựu Tuần 8

- Amazon Bedrock mang đến khả năng tích hợp các mô hình Generative AI hàng đầu một cách an toàn và không cần quản lý máy chủ GPU phức tạp.
- Kỹ thuật Prompt Engineering kết hợp schema JSON rõ ràng là chìa khóa để trích xuất dữ liệu chính xác từ tài liệu không có cấu trúc.
- Áp dụng vào Tindy: Lập trình giao diện AI Studio trên React; hỗ trợ tải CV PDF lên và hiển thị danh sách kỹ năng được mô hình Bedrock gợi ý để người dùng chọn lựa.
