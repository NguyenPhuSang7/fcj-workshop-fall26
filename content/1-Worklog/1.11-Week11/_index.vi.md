---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Cùng team thống nhất phạm vi sản phẩm gọn hơn.
* Làm giao diện web RoomLedger dùng được cả trên điện thoại lẫn máy tính.

### Các công việc đã triển khai trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Review và merge PR #36 (tăng bộ nhớ Lambda RenderPdf và EvidenceSeal lên 512 MB) <br> - Cùng team thu gọn phạm vi còn đồng hồ và hoá đơn: chỉ chủ nhà tải ảnh đồng hồ, người thuê được xem ảnh, bỏ phần trả phòng và quyết toán | 23/11/2026 | 23/11/2026 | |
| 3 | - Chốt chỉ làm web, không làm app native; người thuê dùng được cả trên máy tính <br> - Dựng design system, layout responsive, màn hình duyệt chỉ số đồng hồ và hoá đơn cho người thuê <br> - Làm nốt các màn hình còn lại cho chủ nhà, người thuê và trang public trên dữ liệu mẫu | 24/11/2026 | 24/11/2026 | |
| 4 | - Sửa các lỗi phát hiện khi test: điều hướng của chủ nhà trên điện thoại, toast hoàn tác, nút chụp lại ảnh, chặn duyệt chỉ số hai lần, phóng to ảnh và link khiếu nại cho người thuê, cùng một số chỗ về câu chữ và accessibility | 25/11/2026 | 25/11/2026 | |
| 5 | - (Dự kiến) Mở pull request cho phần giao diện và xử lý review | 26/11/2026 | | |
| 6 | - (Dự kiến) Tiếp tục chỉnh giao diện theo góp ý của team | 27/11/2026 | | |

### Kết quả đạt được tuần 11:

* Nhóm đã có phạm vi rõ ràng và gọn hơn: chỉ số đồng hồ và hoá đơn.
* Toàn bộ màn hình RoomLedger cho chủ nhà, người thuê và trang public đã chạy trên dữ liệu mẫu, cả điện thoại lẫn máy tính.

### Khó khăn & cách giải quyết:

* Phạm vi mới không còn phần trả phòng và quyết toán mà mình làm ở tuần 9 và 10. Mình chuyển sang làm frontend, chỗ team đang cần thêm người.

### Kế hoạch tuần tới:

* Nối giao diện với API thật.
* Chuẩn bị cho buổi demo cuối kỳ.
