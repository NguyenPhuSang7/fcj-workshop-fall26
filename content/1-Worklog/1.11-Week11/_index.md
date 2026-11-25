---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Agree on a smaller product scope with the team.
* Build the RoomLedger web screens so they work on both phone and desktop.

### Tasks carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Review and merge PR #36 (RenderPdf and EvidenceSeal Lambdas set to 512 MB) <br> - Narrow the scope with the team to meters and invoices: only the landlord uploads meter photos, the tenant can view them, move-out and settlement are out | 23/11/2026 | 23/11/2026 | |
| 3 | - Decide on a web app only, no native app; tenants can use it on desktop too <br> - Build the design system, the responsive layouts, the meter review screen and the tenant invoice <br> - Build the rest of the landlord, tenant and public screens on sample data | 24/11/2026 | 24/11/2026 | |
| 4 | - Fix what came up in testing: landlord navigation on phone, the undo toast, the retake photo button, approving a meter reading twice, photo zoom and the dispute link for tenants, plus copy and accessibility fixes | 25/11/2026 | 25/11/2026 | |
| 5 | - (Planned) Open a pull request for the web screens and work through the review | 26/11/2026 | | |
| 6 | - (Planned) Keep fixing the screens based on team feedback | 27/11/2026 | | |

### Week 11 Achievements:

* The team now has a clear and smaller scope: meter readings and invoices.
* Every RoomLedger screen for landlords, tenants and public pages runs on sample data, on both phone and desktop.

### Difficulties & Solutions:

* The new scope left out the move-out and settlement work I did in weeks 9 and 10. I moved over to the frontend, where the team needed more hands.

### Plan for next week:

* Connect the screens to the real API.
* Get ready for the final demo.
