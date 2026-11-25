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
| 1 | **Kiến thức và kỹ năng chuyên môn** | Em làm chủ kiến trúc Frontend React/TypeScript/Tailwind CSS, tích hợp API RESTful và SignalR WebSocket real-time chat. Em áp dụng kiến thức AWS để tối ưu phân phối client tĩnh qua S3 + CloudFront (OAC) và cấu hình chính sách CORS, cơ chế Rate Limiting bảo vệ backend. | ✅ |  |  |
| 2 | **Khả năng học hỏi** | Em hoàn thành đều đặn nhật ký học AWS Cloud Practitioner Essentials 13 tuần. Khi tiếp cận công nghệ mới như Amazon Bedrock hay SignalR, em chủ động tìm hiểu tài liệu chính thức và áp dụng vào giao diện duyệt bản nháp hồ sơ AI. | ✅ |  |  |
| 3 | **Tính chủ động** | Em chủ động thiết kế UI/UX theo hướng hiện đại, xây dựng hệ thống component tái sử dụng, đồng thời phát hiện sớm nguy cơ spam tin nhắn chat để đề xuất triển khai middleware Rate Limiting ở Backend. | ✅ |  |  |
| 4 | **Tinh thần trách nhiệm** | Em cam kết hoàn thành đúng tiến độ các màn hình theo từng sprint (Auth, Profile, Project Discovery, Chat). Khi gặp lỗi trình duyệt chặn gọi API trên domain CloudFront, em kiên trì debug đến khi giải quyết triệt để vấn đề CORS. | ✅ |  |  |
| 5 | **Kỷ luật** | Em tuân thủ thời gian học tập, họp nhóm định kỳ và quy chuẩn commit Git. Em cần cải thiện việc ghi chép nhật ký thường xuyên hơn trong những tuần cao điểm tích hợp tính năng. |  | ✅ |  |
| 6 | **Tinh thần cầu tiến** | Em luôn lắng nghe phản hồi từ mentor và đồng đội để tinh chỉnh trải nghiệm người dùng, sửa đổi DTO và tối ưu hóa luồng tương tác Interested/Accept. | ✅ |  |  |
| 7 | **Giao tiếp** | Em chủ động trao đổi với thành viên phụ trách Backend và Hạ tầng để thống nhất contract API, format dữ liệu JSON và cơ chế authentication token. | ✅ |  |  |
| 8 | **Hợp tác nhóm** | Em phối hợp ăn ý với nhóm trong các đợt merge pull request giữa frontend và backend, đồng thời cùng nhóm diễn tập quy trình deploy CI/CD và kiểm thử kịch bản nghiệm thu. | ✅ |  |  |
| 9 | **Ứng xử chuyên nghiệp** | Em tôn trọng quy tắc bảo mật dữ liệu, không hardcode secret hay API keys trên mã nguồn Frontend, và chuẩn bị kịch bản kiểm thử rõ ràng, khách quan. | ✅ |  |  |
| 10 | **Tư duy giải quyết vấn đề** | Khi gặp lỗi nâng cấp giao thức WebSocket qua CloudFront, em sử dụng DevTools Network để phân tích header và cùng nhóm rà soát cấu hình CloudFront VPC Origin và ALB listener để khắc phục thành công mã 101. | ✅ |  |  |
| 11 | **Đóng góp vào dự án và cộng đồng** | Đóng góp toàn bộ tầng giao diện tương tác của Tindy, luồng realtime chat SignalR, cấu hình CORS, cơ chế chống spam chat Rate Limiting, và tập trung hoàn thành đúng tiến độ các mục tiêu phát triển dự án nhóm. | ✅ |  |  |
| 12 | **Tổng thể** | Em đánh giá bản thân đã hoàn thành xuất sắc mục tiêu thực tập, vừa củng cố vững chắc kỹ năng Frontend/Fullstack, vừa mở rộng đáng kể hiểu biết thực tế về điện toán đám mây AWS. | ✅ |  |  |

---

### Điểm cần cải thiện cho tương lai

1. **Đào sâu hơn vào Infrastructure as Code (IaC):** Em muốn tự tay viết và tùy biến các template CloudFormation/Terraform một cách độc lập thay vì chỉ tập trung vào mã nguồn ứng dụng và cấu hình phân phối tĩnh.
2. **Nâng cao kỹ năng kiểm thử tự động (E2E Testing):** Trong dự án tới, em dự định áp dụng Cypress hoặc Playwright để tự động hóa toàn bộ các kịch bản kiểm thử giao diện trong pipeline CI/CD.
3. **Quản lý state client phức tạp hơn:** Tiếp tục nghiên cứu các mô hình quản lý state phân tán và caching dữ liệu offline cho ứng dụng Progressive Web App (PWA).
