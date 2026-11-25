---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Learn how networking works on AWS: VPC, Security Groups, NACLs, Internet Gateway and NAT Gateway.
* Build a multi-tier network by hand.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - VPC concepts and setup <br>&emsp; + CIDR blocks, public and private subnets, route tables | 28/09/2026 | 28/09/2026 | <https://000003.awsfcaj.com/> |
| 3 | - Join the AWS Cloud Day And AI Day Hanoi watch party | 29/09/2026 | 29/09/2026 | |
| 4 | - Compare Security Groups with NACLs <br> - Learn what the Internet Gateway and NAT Gateway are for | 30/09/2026 | 30/09/2026 | <https://000003.awsfcaj.com/> <br> <https://000092.awsfcaj.com/> |
| 5 | - Lab: multi-tier network <br>&emsp; + Create a VPC with one public and one private subnet <br>&emsp; + Attach an Internet Gateway and add a route for the public subnet <br>&emsp; + Add a NAT Gateway so the private subnet can reach the Internet <br>&emsp; + Give the web tier and the app tier their own Security Group, then test traffic between them <br>&emsp; + Clean up everything afterwards | 01/10/2026 | 01/10/2026 | <https://000092.awsfcaj.com/> |
| 6 | - Join the Fireside Chat with Dr. Werner Vogels | 02/10/2026 | 02/10/2026 | |

### Week 3 Achievements:

* I can lay out a network on AWS with a VPC, public and private subnets and route tables.
* I know the difference between a Security Group (works on the instance, stateful) and a NACL (works on the subnet, stateless).
* I understand what the Internet Gateway does and what the NAT Gateway does.
* I built a working multi-tier network inside a VPC.

### Difficulties & Solutions:

* The events covered a lot of case studies from big companies, but there wasn't enough time for me to follow all of them.

### Plan for next week:

* IAM is next on the AWS Free Tier roadmap: users, groups, roles, policies and MFA.
