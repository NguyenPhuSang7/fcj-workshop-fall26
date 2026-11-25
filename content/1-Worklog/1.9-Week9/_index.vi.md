---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Làm luồng trả phòng và chỉ số đồng hồ lúc nhận phòng cho dự án nhóm RoomLedger.
* Viết blog 1 và chọn chủ đề cho blog 2, blog 3.

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Ôn lại CloudWatch <br> - Làm việc nhóm: tiếp tục dự án | 09/11/2026 | 09/11/2026 | |
| 3 | - Viết blog 1 <br> - RoomLedger trả phòng (MD-06): <br>&emsp; + Mở biên bản trả phòng và gửi đi so sánh <br>&emsp; + Dùng perceptual hash để bỏ qua các cặp ảnh gần như không đổi <br>&emsp; + So sánh ảnh bằng Bedrock, Sonnet lỗi thì chuyển sang Haiku <br>&emsp; + Chủ nhà duyệt các phát hiện, người thuê đồng ý hoặc khiếu nại | 10/11/2026 | 10/11/2026 | <https://aws.amazon.com/blogs/architecture/modernization-pathways-for-a-legacy-net-framework-monolithic-application-on-aws/> <br> <https://www.facebook.com/groups/awsstudygroupfcj/posts/2333637697401189> |
| 4 | - Lên ý tưởng cho blog 2 <br> - RoomLedger nhận phòng (MD-04): phải nhập chỉ số điện, nước ban đầu thì mới xác nhận được biên bản <br> - Sửa các trường hợp reviewer chỉ ra ở PR #15 | 11/11/2026 | 11/11/2026 | <https://builder.aws.com/> |
| 5 | - Bắt đầu viết blog 3 về tối ưu chi phí trên AWS <br> - Làm việc nhóm: áp dụng những gì đọc được trong tài liệu blog vào dự án | 12/11/2026 | 12/11/2026 | <https://builder.aws.com/> <br> <https://cloudjourney.awsfcaj.com/> |
| CN | - Từ chối ảnh gửi tới sau khi biên bản đã khoá <br> - Chuyển phần so sánh trả phòng thành state machine Step Functions, có DLQ và alarm <br> - Merge PR #15 và #18 | 15/11/2026 | 15/11/2026 | |

### Kết quả đạt được tuần 9:

* Đã viết xong blog 1 và đăng lên group FCJ.
* Luồng trả phòng chạy được trọn vẹn ở backend, từ lúc mở biên bản tới lúc người thuê phản hồi.
* Lần đầu mình dùng Bedrock, và bài lab Step Functions ở tuần 6 giúp ích nhiều khi dựng state machine so sánh ảnh.

### Khó khăn & cách giải quyết:

* Review ở PR #15 chỉ ra những trường hợp mình chưa nghĩ tới, ví dụ hợp đồng thuê đã quyết toán hoặc chỉ số đồng hồ đã được xác nhận. Mình sửa và bổ sung test ngay trong ngày.

### Kế hoạch tuần tới:

* Hoàn thành blog 2 và viết tiếp blog 3.
* Làm phần quyết toán trả phòng cho RoomLedger.
