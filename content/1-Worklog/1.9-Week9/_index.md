---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Build the move-out flow and the move-in meter readings for our team project, RoomLedger.
* Write blog 1 and pick topics for blogs 2 and 3.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Go back over CloudWatch <br> - Team work on the project | 09/11/2026 | 09/11/2026 | |
| 3 | - Write blog 1 <br> - RoomLedger move-out (MD-06): <br>&emsp; + Open a move-out inspection and submit it for comparison <br>&emsp; + Perceptual hash to skip photo pairs that barely changed <br>&emsp; + Compare photos with Bedrock, falling back from Sonnet to Haiku <br>&emsp; + Landlord reviews the findings, tenant accepts or disputes them | 10/11/2026 | 10/11/2026 | <https://aws.amazon.com/blogs/architecture/modernization-pathways-for-a-legacy-net-framework-monolithic-application-on-aws/> <br> <https://www.facebook.com/groups/awsstudygroupfcj/posts/2333637697401189> |
| 4 | - Brainstorm topics for blog 2 <br> - RoomLedger move-in (MD-04): opening electricity and water readings are required before the inspection can be confirmed <br> - Fix the cases the reviewer found on PR #15 | 11/11/2026 | 11/11/2026 | <https://builder.aws.com/> |
| 5 | - Start blog 3 on cost optimization on AWS <br> - Team work: apply ideas from the blog sources to the project | 12/11/2026 | 12/11/2026 | <https://builder.aws.com/> <br> <https://cloudjourney.awsfcaj.com/> |
| Sun | - Reject photos that arrive after an inspection is locked <br> - Move-out compare as a Step Functions state machine, with a DLQ and alarms <br> - Merge PRs #15 and #18 | 15/11/2026 | 15/11/2026 | |

### Week 9 Achievements:

* Blog 1 is written and posted in the FCJ group.
* The move-out flow works end to end on the backend, from opening the inspection to the tenant's answer.
* I used Bedrock for the first time, and the Step Functions lab from week 6 helped a lot when I built the compare state machine.

### Difficulties & Solutions:

* The review on PR #15 found cases I hadn't thought about, such as a tenancy that is already settled or a meter reading that is already confirmed. I fixed them and added tests the same day.

### Plan for next week:

* Finish blog 2 and keep going with blog 3.
* Build the move-out settlement for RoomLedger.
