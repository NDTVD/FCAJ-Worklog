---
title: "Tự đánh giá"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

# Bản tự đánh giá kết quả thực tập

Trong chương trình **First Cloud AI Journey (FCAJ)**, em (**Cao Thành Nhân**) đã hoàn thành việc học tập các kiến thức nền tảng điện toán đám mây qua khóa **AWS Cloud Practitioner Essentials**, đồng thời trực tiếp đảm nhận vai trò **Kỹ sư Frontend (React / TypeScript / Tailwind CSS)** và hỗ trợ tối ưu **Backend (CORS, Message Rate Limiting)** cho dự án **Tindy**. 

Báo cáo ghi nhận ba đầu ra trọng tâm của em là [nhật ký học tập Worklog 13 tuần](/vi/1-worklog/), [bản đề xuất kỹ thuật Tindy](/vi/2-proposal/), và [kịch bản kiểm thử giao diện & video demo Workshop 5.6](/vi/5-workshop/5.6-application-demo/).

---

### Đánh giá theo tiêu chí

| STT | Tiêu chí | Căn cứ tự đánh giá của cá nhân | Tốt | Khá | Trung bình |
| :---: | :--- | :--- | :---: | :---: | :---: |
| 1 | **Kiến thức và kỹ năng chuyên môn** | Nắm vững kỹ thuật lập trình giao diện React/TypeScript/Tailwind CSS và kết nối API RESTful. Đã tiếp thu tốt các kiến thức nền tảng đám mây qua khóa học, tuy nhiên vẫn cần tích lũy thêm kinh nghiệm thực chiến về kiến trúc hệ thống backend phân tán và hạ tầng AWS nâng cao. |  | ✅ |  |
| 2 | **Khả năng học hỏi** | Hoàn thành đều đặn nội dung học AWS Cloud Practitioner Essentials 13 tuần. Khi tiếp cận công nghệ mới như Amazon Bedrock hay SignalR, em chủ động tìm hiểu tài liệu chính thức và áp dụng hiệu quả vào giao diện duyệt hồ sơ AI. | ✅ |  |  |
| 3 | **Tính chủ động** | Chủ động thiết kế hệ thống component UI tái sử dụng và đề xuất giải pháp Rate Limiting cho chat. Tuy nhiên ở các cấu hình hạ tầng phức tạp đa tầng, em vẫn cần tham khảo thêm ý kiến định hướng từ mentor và đồng đội. |  | ✅ |  |
| 4 | **Tinh thần trách nhiệm** | Cam kết hoàn thành đúng tiến độ các màn hình theo từng sprint (Auth, Profile, Project Discovery, Chat). Kiên trì tìm hiểu và debug đến khi giải quyết triệt để lỗi chặn kết nối CORS trên domain CloudFront. | ✅ |  |  |
| 5 | **Kỷ luật** | Luôn tuân thủ thời gian học tập, tham gia đầy đủ các buổi họp nhóm và tuân thủ quy chuẩn commit Git. Cần duy trì việc ghi chép nhật ký công việc đều đặn hơn trong các giai đoạn cao điểm chạy dự án. |  | ✅ |  |
| 6 | **Tinh thần cầu tiến** | Luôn cầu thị và sẵn sàng tiếp thu các ý kiến đóng góp mang tính xây dựng từ mentor và đồng đội để tinh chỉnh trải nghiệm người dùng, sửa đổi DTO và tối ưu hóa luồng tương tác. | ✅ |  |  |
| 7 | **Giao tiếp** | Trao đổi rõ ràng, đúng trọng tâm với thành viên phụ trách Backend về contract API và cấu trúc dữ liệu. Tiếp tục rèn luyện kỹ năng truyền đạt ngắn gọn và chuẩn hóa tài liệu kỹ thuật trong làm việc nhóm. |  | ✅ |  |
| 8 | **Hợp tác nhóm** | Phối hợp nhịp nhàng với nhóm trong các đợt merge pull request, cùng đồng đội diễn tập quy trình deploy CI/CD và kiểm thử các kịch bản nghiệm thu. | ✅ |  |  |
| 9 | **Ứng xử chuyên nghiệp** | Tôn trọng nghiêm ngặt các quy tắc bảo mật dữ liệu, không hardcode credentials hay API keys trong mã nguồn client, và xây dựng các ca kiểm thử khách quan. | ✅ |  |  |
| 10 | **Tư duy giải quyết vấn đề** | Đã khắc phục thành công sự cố CORS và nâng cấp giao thức WebSocket qua DevTools, đồng thời nhận thức được việc giải quyết các sự cố hạ tầng đám mây phức tạp cần sự phối hợp đa chiều với đồng đội. |  | ✅ |  |
| 11 | **Đóng góp vào dự án và cộng đồng** | Đóng góp hoàn chỉnh tầng giao diện người dùng của Tindy, tích hợp chat realtime SignalR, cấu hình CORS, giải pháp chống spam chat Rate Limiting, và nỗ lực vì mục tiêu chung của nhóm. |  | ✅ |  |
| 12 | **Tổng thể** | Đạt mức hoàn thành tốt các mục tiêu đề ra trong kỳ thực tập. Nâng cao rõ rệt năng lực lập trình Frontend và xây dựng được nền tảng tư duy kiến trúc đám mây AWS thực tế với tinh thần khiêm tốn, sẵn sàng học hỏi. |  | ✅ |  |

---

### Điểm cần cải thiện cho tương lai

1. **Đào sâu hơn vào Infrastructure as Code (IaC):** Em muốn tự tay viết và tùy biến các template CloudFormation/Terraform một cách độc lập thay vì chỉ tập trung vào mã nguồn ứng dụng và cấu hình phân phối tĩnh.
2. **Nâng cao kỹ năng kiểm thử tự động (E2E Testing):** Trong dự án tới, em dự định áp dụng Cypress hoặc Playwright để tự động hóa toàn bộ các kịch bản kiểm thử giao diện trong pipeline CI/CD.
3. **Quản lý state client phức tạp hơn:** Tiếp tục nghiên cứu các mô hình quản lý state phân tán và caching dữ liệu offline cho ứng dụng Progressive Web App (PWA).
