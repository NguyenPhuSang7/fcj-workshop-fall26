---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Publish blog 2 and get blog 3 through review.
* Finish the move-out settlement for RoomLedger and add monitoring to the project.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Finish blog 2 (securing a legacy .NET application on AWS) and post it in the FCJ group <br> - Collect material for blog 3 | 16/11/2026 | 16/11/2026 | <https://www.facebook.com/groups/awsstudygroupfcj/posts/2338886330209659> <br> <https://cloudjourney.awsfcaj.com/> |
| 3 | - Research and write blog 3 (cutting costs for a .NET application on AWS) <br> - RoomLedger settlement: <br>&emsp; + Final electricity and water readings are required before move-out can be submitted <br>&emsp; + Refund = deposit minus accepted charges minus unpaid invoices <br>&emsp; + A Lambda renders the settlement record as a PDF <br>&emsp; + Only the tenant can upload move-out photos <br> - Monitoring stack: SNS alarm topic, CloudWatch dashboard, alarms for API 5xx, Lambda throttles and RDS free storage, log retention for the workflow Lambdas | 17/11/2026 | 17/11/2026 | <https://aws.amazon.com/blogs/architecture/how-orderserv-achieved-up-to-64-cost-savings-with-multi-tenant-ecs/> <br> <https://docs.aws.amazon.com/cost-management/latest/userguide/cost-optimization-hub.html> <br> <https://000007.awsfcaj.com> <br> <https://000032.awsfcaj.com> <br> <https://000034.awsfcaj.com> <br> <https://000042.awsfcaj.com> <br> <https://000064.awsfcaj.com> |
| 4 | - Rework the blog 3 diagram and text after review: VPC endpoints for ECR, Secrets Manager and Logs, Scheduled Scaling for dev/test, Fargate Spot, BYOM, cost allocation tags, S3 lifecycle <br> - Team work on the FCAJ project | 18/11/2026 | 18/11/2026 | <https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html> <br> <https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-capacity-providers.html> <br> <https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html> <br> <https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CloudWatch_Logs_Log_Classes.html> <br> <https://cloudjourney.awsfcaj.com/> <br> <https://www.facebook.com/groups/awsstudygroupfcj/posts/2341814056583553> |
| 5 | - Team work on the FCAJ project | 19/11/2026 | 19/11/2026 | |
| 6 | - Integration tests for JWT login, running through the real JwtBearer handler and the group policies | 20/11/2026 | 20/11/2026 | |
| Sun | - Team work on RoomLedger <br> - Infra: RDS Multi-AZ for prod, an SQS queue for photo processing, a prod stage that follows architecture v8.5.2 <br> - Cut features: AI photo comparison at move-out and the unused contract-terms prompt | 22/11/2026 | 22/11/2026 | |

### Week 10 Achievements:

* Blog 2 is published, and blog 3 has been revised once after review.
* Settlement works on the backend: the refund is calculated, the room goes back to vacant and a PDF record is created.
* RoomLedger now has its own CloudWatch dashboard and alarms that send to one SNS topic. This is the week 8 lab, but on a real project.

### Difficulties & Solutions:

* On 22/11 the team cut scope, and the AI photo comparison I built in week 9 was removed. Move-out is now reviewed by hand.

### Plan for next week:

* Start on the RoomLedger web screens.
