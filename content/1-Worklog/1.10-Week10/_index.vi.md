---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Làm xong phần quyết toán trả phòng cho RoomLedger và thêm giám sát cho dự án.
* Viết ba bài blog cho AWS Study Group.

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Làm việc nhóm: tiếp tục project FCAJ | 16/11/2026 | 16/11/2026 | |
| 3 | - RoomLedger quyết toán: <br>&emsp; + Phải có chỉ số điện, nước cuối kỳ mới gửi được biên bản trả phòng <br>&emsp; + Tiền hoàn = tiền cọc trừ các khoản đã đồng ý trừ hoá đơn chưa trả <br>&emsp; + Một Lambda xuất biên bản quyết toán ra PDF <br>&emsp; + Chỉ người thuê được tải ảnh trả phòng lên <br> - Stack giám sát: SNS topic cho alarm, CloudWatch dashboard, alarm cho API 5xx, Lambda bị throttle và dung lượng trống của RDS, thời hạn lưu log cho các Lambda workflow | 17/11/2026 | 17/11/2026 | <https://000008.awsfcaj.com/> |
| 4 | - Làm việc nhóm: tiếp tục project FCAJ | 18/11/2026 | 18/11/2026 | |
| 5 | - Làm việc nhóm: tiếp tục project FCAJ | 19/11/2026 | 19/11/2026 | |
| 6 | - Viết integration test cho đăng nhập JWT, chạy qua JwtBearer thật và các policy theo group | 20/11/2026 | 20/11/2026 | |
| CN | - Viết ba bài blog cho AWS Study Group: <br>&emsp; + [CloudFront + S3 với OAC](../../3-blogsposted/3.1-blog1/) <br>&emsp; + [Lambda trong VPC bị timeout](../../3-blogsposted/3.2-blog2/) <br>&emsp; + [Saga với Step Functions](../../3-blogsposted/3.3-blog3/) <br> - Làm việc nhóm cho RoomLedger: RDS Multi-AZ cho prod, hàng đợi SQS xử lý ảnh, stage prod theo kiến trúc v8.5.2 <br> - Cắt bớt tính năng: so sánh ảnh bằng AI lúc trả phòng và prompt điều khoản hợp đồng không dùng tới | 22/11/2026 | 22/11/2026 | <https://000094.awsfcaj.com/> <br> <https://000111.awsfcaj.com/> <br> <https://000047.awsfcaj.com/> |

### Kết quả đạt được tuần 10:

* Phần quyết toán chạy được ở backend: tính tiền hoàn, chuyển phòng về trạng thái trống và tạo biên bản PDF.
* RoomLedger đã có CloudWatch dashboard và alarm riêng, tất cả gửi về một SNS topic. Đây chính là bài lab tuần 8 nhưng làm trên dự án thật.
* Viết xong ba bài blog. Bài nào cũng bắt đầu từ một lỗi hay gặp (403 sau CloudFront, Lambda trong VPC bị timeout, rollback giữa các microservice) và kết thúc bằng một checklist.

### Khó khăn & cách giải quyết:

* Ngày 22/11 nhóm thu gọn phạm vi, phần so sánh ảnh bằng AI mình làm ở tuần 9 bị bỏ. Trả phòng giờ được duyệt thủ công.

### Kế hoạch tuần tới:

* Bắt tay vào làm giao diện web cho RoomLedger.
