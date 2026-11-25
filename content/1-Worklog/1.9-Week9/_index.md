---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Build the move-out flow and the move-in meter readings for our team project, RoomLedger.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Go back over CloudWatch <br> - Team work on the project | 09/11/2026 | 09/11/2026 | |
| 3 | - RoomLedger move-out (MD-06): <br>&emsp; + Open a move-out inspection and submit it for comparison <br>&emsp; + Perceptual hash to skip photo pairs that barely changed <br>&emsp; + Compare photos with Bedrock, falling back from Sonnet to Haiku <br>&emsp; + Landlord reviews the findings, tenant accepts or disputes them | 10/11/2026 | 10/11/2026 | |
| 4 | - RoomLedger move-in (MD-04): opening electricity and water readings are required before the inspection can be confirmed <br> - Fix the cases the reviewer found on PR #15 | 11/11/2026 | 11/11/2026 | |
| 5 | - Team work on the project | 12/11/2026 | 12/11/2026 | |
| Sun | - Reject photos that arrive after an inspection is locked <br> - Move-out compare as a Step Functions state machine, with a DLQ and alarms <br> - Merge PRs #15 and #18 | 15/11/2026 | 15/11/2026 | <https://000047.awsfcaj.com/> |

### Week 9 Achievements:

* The move-out flow works end to end on the backend, from opening the inspection to the tenant's answer.
* I used Bedrock for the first time, and the Step Functions lab from week 6 helped a lot when I built the compare state machine.

### Difficulties & Solutions:

* The review on PR #15 found cases I hadn't thought about, such as a tenancy that is already settled or a meter reading that is already confirmed. I fixed them and added tests the same day.

### Plan for next week:

* Build the move-out settlement for RoomLedger.
