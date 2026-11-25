---
title: "Các bài blogs đã đăng"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

Đây là các bài blog mình viết cho [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj). Mỗi bài bắt đầu từ một tình huống mình hoặc mọi người xung quanh hay gặp trên AWS, giải thích nguyên nhân, và kết thúc bằng một checklist.

### [CloudFront + S3: bucket để private thì website có chạy được không?](3.1-blog1/)
CloudFront với Origin Access Control phục vụ website từ một S3 bucket private hoàn toàn như thế nào, OAC khác OAI ra sao, và ba lỗi hay dẫn tới 403 AccessDenied: dùng website endpoint của S3 làm origin, refresh trang con của SPA, và object mã hoá bằng SSE-KMS. Bài cũng nói về cache và invalidation khi deploy bản build mới.

### [Lambda gắn vào VPC xong thì gọi API bị timeout: request đã đi đâu?](3.2-blog2/)
Vì sao một Lambda kết nối RDS bình thường lại không gọi được API bên ngoài, Secrets Manager hay SQS sau khi gắn vào VPC, và vì sao chuyển sang public subnet cũng không giúp gì. Bài tách traffic theo đích đến (NAT Gateway, Gateway Endpoint, Interface Endpoint), liệt kê những gì cần kiểm tra khi endpoint vẫn timeout, và đặt câu hỏi function có thật sự cần VPC không.

### [Saga với Step Functions: thanh toán lỗi thì rollback đơn hàng thế nào?](3.3-blog3/)
Thứ gì thay cho ROLLBACK khi đơn hàng, kho và thanh toán nằm ở các service riêng. Bài đi qua saga orchestration bằng Step Functions Standard Workflow, khác nhau giữa Retry và Catch, vì sao retry khiến idempotency trở nên bắt buộc, làm gì khi bước bù trừ cũng lỗi, và cách xử lý việc saga không có isolation.
