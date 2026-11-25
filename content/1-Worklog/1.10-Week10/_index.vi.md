---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Đăng blog 2 và hoàn thiện blog 3 sau phản biện.
* Làm xong phần quyết toán trả phòng cho RoomLedger và thêm giám sát cho dự án.

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Hoàn thành blog 2 (bảo mật ứng dụng .NET legacy trên AWS) và đăng lên group FCJ <br> - Gom tài liệu cho blog 3 | 16/11/2026 | 16/11/2026 | <https://www.facebook.com/groups/awsstudygroupfcj/posts/2338886330209659> <br> <https://cloudjourney.awsfcaj.com/> |
| 3 | - Tìm tài liệu và viết blog 3 (giảm chi phí cho ứng dụng .NET trên AWS) <br> - RoomLedger quyết toán: <br>&emsp; + Phải có chỉ số điện, nước cuối kỳ mới gửi được biên bản trả phòng <br>&emsp; + Tiền hoàn = tiền cọc trừ các khoản đã đồng ý trừ hoá đơn chưa trả <br>&emsp; + Một Lambda xuất biên bản quyết toán ra PDF <br>&emsp; + Chỉ người thuê được tải ảnh trả phòng lên <br> - Stack giám sát: SNS topic cho alarm, CloudWatch dashboard, alarm cho API 5xx, Lambda bị throttle và dung lượng trống của RDS, thời hạn lưu log cho các Lambda workflow | 17/11/2026 | 17/11/2026 | <https://aws.amazon.com/blogs/architecture/how-orderserv-achieved-up-to-64-cost-savings-with-multi-tenant-ecs/> <br> <https://docs.aws.amazon.com/cost-management/latest/userguide/cost-optimization-hub.html> <br> <https://000007.awsfcaj.com> <br> <https://000032.awsfcaj.com> <br> <https://000034.awsfcaj.com> <br> <https://000042.awsfcaj.com> <br> <https://000064.awsfcaj.com> |
| 4 | - Sửa sơ đồ và nội dung blog 3 theo phản biện: VPC endpoint cho ECR, Secrets Manager và Logs, Scheduled Scaling cho dev/test, Fargate Spot, BYOM, cost allocation tag, lifecycle S3 <br> - Làm việc nhóm: chạy project FCAJ | 18/11/2026 | 18/11/2026 | <https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html> <br> <https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-capacity-providers.html> <br> <https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html> <br> <https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CloudWatch_Logs_Log_Classes.html> <br> <https://cloudjourney.awsfcaj.com/> <br> <https://www.facebook.com/groups/awsstudygroupfcj/posts/2341814056583553> |
| 5 | - Làm việc nhóm: tiếp tục project FCAJ | 19/11/2026 | 19/11/2026 | |
| 6 | - Viết integration test cho đăng nhập JWT, chạy qua JwtBearer thật và các policy theo group | 20/11/2026 | 20/11/2026 | |
| CN | - Làm việc nhóm cho RoomLedger <br> - Hạ tầng: RDS Multi-AZ cho prod, thêm hàng đợi SQS xử lý ảnh, thêm stage prod theo kiến trúc v8.5.2 <br> - Cắt bớt tính năng: so sánh ảnh bằng AI lúc trả phòng và prompt điều khoản hợp đồng không dùng tới | 22/11/2026 | 22/11/2026 | |

### Kết quả đạt được tuần 10:

* Blog 2 đã đăng, blog 3 đã sửa xong một vòng theo phản biện.
* Phần quyết toán chạy được ở backend: tính tiền hoàn, chuyển phòng về trạng thái trống và tạo biên bản PDF.
* RoomLedger đã có CloudWatch dashboard và alarm riêng, tất cả gửi về một SNS topic. Đây chính là bài lab tuần 8 nhưng làm trên dự án thật.

### Khó khăn & cách giải quyết:

* Ngày 22/11 nhóm thu gọn phạm vi, phần so sánh ảnh bằng AI mình làm ở tuần 9 bị bỏ. Trả phòng giờ được duyệt thủ công.

### Kế hoạch tuần tới:

* Bắt tay vào làm giao diện web cho RoomLedger.
