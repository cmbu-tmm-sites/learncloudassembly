---
title: "Cloud Zones"
weight: 10
---

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly  cloud zone is a set of resources within a cloud account type such as AWS or vSphere.

{{< img src="/Infrastructure/Configure/Cloud-Zones/cloudzones-display.png" alt="Cloud Zones List" >}}

Cloud zones in a specific account region are where your [cloud templates](Design/Cloud_Templates/) deploy workloads. Each cloud zone is associated with a Cloud Assembly [project](/Infrastructure/Administration/Projects/).

{{< img src="/Infrastructure/Configure/Cloud-Zones/cloudzones-view.png" alt="Cloud Zones" >}}

A cloud zone defines a set of [compute resources](/Infrastructure/Resources/Compute/)  that can be used for provisioning. 
Capability tags are effectively applied to all [compute resources](/Infrastructure/Resources/Compute/)  in this cloud zone, but only in the context of this cloud zone.

{{< img src="/Infrastructure/Configure/Cloud-Zones/cloudzones-summary.png" alt="Cloud Zones Summary" >}}

All [compute resources](/Infrastructure/Resources/Compute/) listed apply to this cloud zone.
 Use the filter to add or remove resources from the list. Only [compute resources](/Infrastructure/Resources/Compute/)  that are not assigned to another zone can be used.

{{< img src="/Infrastructure/Configure/Cloud-Zones/cloudzones-compute.png" alt="Cloud Zones Compute Resources" >}}