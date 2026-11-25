---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Tìm hiểu cách các dịch vụ trên AWS giao tiếp với nhau: SQS, SNS, EventBridge và Step Functions.
* Dựng một luồng xử lý hướng sự kiện nhỏ.

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Gửi nhận message với SQS và SNS | 19/10/2026 | 19/10/2026 | <https://000077.awsfcaj.com/> |
| 3 | - Định tuyến sự kiện với EventBridge | 20/10/2026 | 20/10/2026 | <https://000054.awsfcaj.com/> |
| 4 | - Xây workflow với Step Functions | 21/10/2026 | 21/10/2026 | <https://000047.awsfcaj.com/> |
| 5 | - Lab: kiến trúc hướng sự kiện <br>&emsp; + Tạo SNS topic và SQS queue, cho queue subscribe vào topic <br>&emsp; + Thêm EventBridge rule để định tuyến sự kiện <br>&emsp; + Viết Lambda nhận message từ SQS để xử lý <br>&emsp; + Gửi một sự kiện thử và theo dõi nó đi hết luồng <br>&emsp; + Dọn tài nguyên | 22/10/2026 | 22/10/2026 | <https://000054.awsfcaj.com/> <br> <https://000083.awsfcaj.com/> |
| 6 | - Ôn lại phần tích hợp ứng dụng <br> - Tiếp tục làm ý tưởng dự án | 23/10/2026 | 23/10/2026 | |

### Kết quả đạt được tuần 6:

* Giải thích được khi nào dùng SQS (hàng đợi) và khi nào dùng SNS (publish/subscribe).
* Biết EventBridge định tuyến sự kiện ra sao và Step Functions nối các bước thành workflow thế nào.
* Dựng được một luồng hướng sự kiện đơn giản chạy từ đầu đến cuối.

### Khó khăn & cách giải quyết:

* Nhóm đã có ý tưởng nhưng khó ở chỗ hiện thực: chi phí chạy dự án còn cao hơn chi phí mà vấn đề đang gây ra cho người dùng.

### Kế hoạch tuần tới:

* Học container và orchestration theo roadmap AWS Free Tier: Docker, ECS và ECR.
