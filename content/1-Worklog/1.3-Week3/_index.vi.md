---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Hiểu cách mạng hoạt động trên AWS: VPC, Security Group, NACL, Internet Gateway và NAT Gateway.
* Tự tay dựng một mạng nhiều tầng (multi-tier).

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Khái niệm và cách thiết lập VPC <br>&emsp; + Dải CIDR, subnet public và private, route table | 28/09/2026 | 28/09/2026 | <https://000003.awsfcaj.com/> |
| 3 | - Tham dự watch party AWS Cloud Day And AI Day Hanoi | 29/09/2026 | 29/09/2026 | |
| 4 | - So sánh Security Group với NACL <br> - Tìm hiểu Internet Gateway và NAT Gateway dùng để làm gì | 30/09/2026 | 30/09/2026 | <https://000003.awsfcaj.com/> <br> <https://000092.awsfcaj.com/> |
| 5 | - Lab: mạng nhiều tầng <br>&emsp; + Tạo VPC gồm một subnet public và một subnet private <br>&emsp; + Gắn Internet Gateway và thêm route cho subnet public <br>&emsp; + Thêm NAT Gateway để subnet private ra được Internet <br>&emsp; + Tạo Security Group riêng cho tầng web và tầng ứng dụng, rồi thử kết nối giữa hai tầng <br>&emsp; + Dọn hết tài nguyên sau khi làm xong | 01/10/2026 | 01/10/2026 | <https://000092.awsfcaj.com/> |
| 6 | - Tham dự Fireside Chat with Dr. Werner Vogels | 02/10/2026 | 02/10/2026 | |

### Kết quả đạt được tuần 3:

* Biết cách chia mạng trên AWS bằng VPC, subnet public/private và route table.
* Phân biệt được Security Group (gắn với instance, stateful) và NACL (gắn với subnet, stateless).
* Hiểu Internet Gateway và NAT Gateway mỗi cái làm nhiệm vụ gì.
* Dựng được một mạng nhiều tầng chạy thật trong VPC.

### Khó khăn & cách giải quyết:

* Các sự kiện có rất nhiều case study của công ty lớn, nhưng thời gian ngắn nên mình chưa theo kịp hết.

### Kế hoạch tuần tới:

* Học tiếp IAM theo roadmap AWS Free Tier: user, group, role, policy và MFA.
