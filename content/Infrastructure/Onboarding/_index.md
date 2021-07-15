---
title: "Onboarding"
weight: 30
---

## OnBoarding Plans

You use a workload onboarding plan to identify machines that have been data-collected from a /Infrastructure/Connections/Cloud-Accounts/ type in a target region or data center but that are not yet managed by a [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly project.

When you add a /Infrastructure/Connections/Cloud-Accounts/ that contains machines that were deployed outside of [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly, the machines are not managed by Cloud Assembly until you onboard them. Use an onboarding plan to bring unmanaged machines into [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly management. You create a plan, populate it with machines, and then run the plan to import the machines. Using the onboarding plan, you can create a [Cloud Template](/Design/Cloud_Templates/) and can also create one or many [deployments](/Deployments/).

You can onboard one or many unmanaged machines in a single plan by selecting machines manually.

1. You can onboard up to 3,500 unmanaged machines within a single onboarding plan per hour.
2. You can onboard up to 17,000 unmanaged machines concurrently within multiple onboarding plans per hour.

Machines that are available for workload onboarding are listed on the [Resources Machines](/Infrastructure/Resources/Machines/) page relative to a specific /Infrastructure/Connections/Cloud-Accounts/ type and region and labeled as Discovered in the Origin column. Only machines that have been data-collected are listed. After you onboard the machines, they appear in the Origin column as Deployed.

{{< img src="/Infrastructure/Onboarding/onboarding-view.png" alt="Onboarding Plans " >}}

Onboarding also supports onboarding custom properties, attached disks, changing deployment owners, and vSphere networks.

1. <b>Custom properties</b> - you can set custom properties at the plan and at the individual machine levels. A custom property set at the machine level overrides the same property on the plan level.
2. <b>Attached disks</b> - If a machine has any non-bootable disks, they are automatically onboarded with the parent machine. To view non-bootable disks, click the machine name in the plan, and then navigate to the Storage tab.
3. <b>Deployment ownership</b> - Onboarding allows you to change the default deployment owner. To change the owner, select a deployment from the Deployment tab, click Edit owner, and select the desired user associated with the project.

{{< img src="/Infrastructure/Onboarding/onboarding-properties.png" alt="Onboarding Plans " >}}

