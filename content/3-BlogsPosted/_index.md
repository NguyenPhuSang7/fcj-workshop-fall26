---
title: "Blogs Posted"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

These are the blog posts I wrote for the [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj). Each one starts from a problem I or people around me ran into on AWS, explains the cause, and ends with a checklist. The posts were written in Vietnamese; the English pages are translations.

### [CloudFront + S3: can a website run from a private bucket?](3.1-blog1/)
How CloudFront with Origin Access Control serves a website from an S3 bucket that stays fully private, how OAC differs from the older OAI, and the three mistakes that usually end in 403 AccessDenied: using the S3 website endpoint as the origin, refreshing a sub-page of an SPA, and objects encrypted with SSE-KMS. It also covers caching and invalidation when deploying a new build.

### [My Lambda times out after I put it in a VPC: where did the request go?](3.2-blog2/)
Why a Lambda that reaches RDS fine suddenly can't call external APIs, Secrets Manager or SQS once it's attached to a VPC, and why moving it to a public subnet doesn't help. The post splits traffic by destination (NAT Gateway, Gateway Endpoint, Interface Endpoint), lists what to check when an endpoint still times out, and asks whether the function needs a VPC at all.

### [Saga with Step Functions: how do you roll back an order when payment fails?](3.3-blog3/)
What replaces ROLLBACK once orders, inventory and payments live in separate services. The post walks through saga orchestration with a Step Functions Standard Workflow, the difference between Retry and Catch, why retries make idempotency necessary, what to do when a compensating step fails, and how to deal with a saga having no isolation.
