---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Learn how services talk to each other on AWS: SQS, SNS, EventBridge and Step Functions.
* Build a small event-driven setup.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Messaging with SQS and SNS | 19/10/2026 | 19/10/2026 | <https://000077.awsfcaj.com/> |
| 3 | - Routing events with EventBridge | 20/10/2026 | 20/10/2026 | <https://000054.awsfcaj.com/> |
| 4 | - Building workflows with Step Functions | 21/10/2026 | 21/10/2026 | <https://000047.awsfcaj.com/> |
| 5 | - Lab: event-driven architecture <br>&emsp; + Create an SNS topic and an SQS queue, then subscribe the queue to the topic <br>&emsp; + Add an EventBridge rule to route the events <br>&emsp; + Write a Lambda function that picks up messages from SQS <br>&emsp; + Send a test event and follow it through the whole flow <br>&emsp; + Clean up the resources | 22/10/2026 | 22/10/2026 | <https://000054.awsfcaj.com/> <br> <https://000083.awsfcaj.com/> |
| 6 | - Review application integration <br> - Keep working on the project idea | 23/10/2026 | 23/10/2026 | |

### Week 6 Achievements:

* I can explain when to use SQS (a queue) and when to use SNS (publish/subscribe).
* I know how EventBridge routes events and how Step Functions chains steps into a workflow.
* I built a simple event-driven flow from end to end.

### Difficulties & Solutions:

* We finally have an idea, but making it real is the hard part: running the project would cost more than the problem costs people today.

### Plan for next week:

* Containers and orchestration from the AWS Free Tier roadmap: Docker, ECS and ECR.
