---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Finish the move-out settlement for RoomLedger and add monitoring to the project.
* Write my three blog posts for the AWS Study Group.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Team work on the FCAJ project | 16/11/2026 | 16/11/2026 | |
| 3 | - RoomLedger settlement: <br>&emsp; + Final electricity and water readings are required before move-out can be submitted <br>&emsp; + Refund = deposit minus accepted charges minus unpaid invoices <br>&emsp; + A Lambda renders the settlement record as a PDF <br>&emsp; + Only the tenant can upload move-out photos <br> - Monitoring stack: SNS alarm topic, CloudWatch dashboard, alarms for API 5xx, Lambda throttles and RDS free storage, log retention for the workflow Lambdas | 17/11/2026 | 17/11/2026 | <https://000008.awsfcaj.com/> |
| 4 | - Team work on the FCAJ project | 18/11/2026 | 18/11/2026 | |
| 5 | - Team work on the FCAJ project | 19/11/2026 | 19/11/2026 | |
| 6 | - Integration tests for JWT login, running through the real JwtBearer handler and the group policies | 20/11/2026 | 20/11/2026 | |
| Sun | - Write three blog posts for the AWS Study Group: <br>&emsp; + [CloudFront + S3 with OAC](../../3-blogsposted/3.1-blog1/) <br>&emsp; + [Lambda in a VPC timing out](../../3-blogsposted/3.2-blog2/) <br>&emsp; + [Saga with Step Functions](../../3-blogsposted/3.3-blog3/) <br> - Team work on RoomLedger: RDS Multi-AZ for prod, an SQS queue for photo processing, a prod stage that follows architecture v8.5.2 <br> - Cut features: AI photo comparison at move-out and the unused contract-terms prompt | 22/11/2026 | 22/11/2026 | <https://000094.awsfcaj.com/> <br> <https://000111.awsfcaj.com/> <br> <https://000047.awsfcaj.com/> |

### Week 10 Achievements:

* Settlement works on the backend: the refund is calculated, the room goes back to vacant and a PDF record is created.
* RoomLedger now has its own CloudWatch dashboard and alarms that send to one SNS topic. This is the week 8 lab, but on a real project.
* I wrote three blog posts. Each one starts from a problem that comes up a lot (403 behind CloudFront, a Lambda that times out in a VPC, rolling back across microservices) and ends with a checklist.

### Difficulties & Solutions:

* On 22/11 the team cut scope, and the AI photo comparison I built in week 9 was removed. Move-out is now reviewed by hand.

### Plan for next week:

* Start on the RoomLedger web screens.
