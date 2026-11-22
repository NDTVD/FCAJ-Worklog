---
title: "Workshop"
date: 2026-11-18
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

Triển khai lại hạ tầng **Tindy trên AWS bằng CloudFormation**, tạo database PostgreSQL mới, chạy migration và seed dữ liệu demo, sau đó kiểm tra và quay video sử dụng ứng dụng qua CloudFront.

Workshop dùng sáu template `foundation.yaml`, `network.yaml`, `database.yaml`, `integrations.yaml`, `runtime.yaml` và `edge.yaml`. Mỗi phần giải thích tài nguyên, tham số đầu vào, Outputs dùng cho stack tiếp theo và kết quả cần kiểm tra. Ảnh được chụp ngay tại các mốc thực hành.

## Cấu trúc đã chốt

| Mục | Nội dung |
| --- | --- |
| [5.1 Tổng quan kiến trúc](5.1-Overview/) | Kiến trúc Tindy, sáu template và mục tiêu. |
| [5.2 Chuẩn bị triển khai](5.2-Prerequisites/) | AWS, CLI, source, image và mapping. |
| [5.3 Foundation và Network](5.3-Foundation-Network/) | Import Foundation và triển khai mạng. |
| [5.4 Database và Integrations](5.4-Database-Integrations/) | Database Fresh và tích hợp quét PDF. |
| [5.5 Runtime, seed và Edge](5.5-Runtime-Edge/) | Edge maintenance, Runtime, bootstrap, migration, seed và mở traffic. |
| [5.6 Kiểm tra và demo ứng dụng](5.6-Verification-Demo/) | Kiểm tra giao diện React, tích hợp API, SignalR chat, CORS và Rate Limiting. |
| [5.7 Dọn dẹp tài nguyên](5.7-Cleanup/) | Cleanup môi trường hiện tại cùng ảnh và trạng thái đã xác minh. |

## Lượt thực hành hiện tại

Hệ thống đã tồn tại nên thực hành mở đầu bằng cleanup, được ghi ở mục 5.7 theo cấu trúc bài viết. Sau đó dựng lại sáu stack trong cùng môi trường, chọn database Fresh, seed dữ liệu demo và dùng hostname CloudFront mới.

Đã xác minh maintenance trước cleanup và xóa thành công cả sáu stack Runtime, Database, Integrations, Edge, Network và Foundation với trạng thái DELETE_COMPLETE. Hướng dẫn chi tiết và ảnh nằm ở mục 5.7.
