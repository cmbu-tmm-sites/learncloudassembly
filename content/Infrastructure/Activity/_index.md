---
title: "Activity"
weight: 50
---

Your deployment request might fail for many reasons. It might be due to network traffic, a lack of resources on the target cloud provider, or a flawed deployment specification, perhaps the deployment succeeded, but it does not appear to be working.

Use the <strong> Activity </strong> tab to examine your deployment [Requests](/Infrastructure/Activity/Requests/), review any error messages, and determine whether the problem is the environment, the requested workload specification, or something else.
You use this [Event Logs](/Infrastructure/Activity/Events-Log/)to begin your investigation.
The process might reveal that the failure was due to a transient environmental problem. Redeploying the request after verifying the conditions have improved resolves this type of problem.