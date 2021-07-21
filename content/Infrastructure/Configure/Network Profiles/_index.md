---
title: "Network Profiles"
weight: 60
---

A [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud network profile describes the behavior of the network to be deployed.

For example, a network might need to be Internet-facing rather than internal-only.
[Networks](/Infrastructure/Resources/Networks/) and network profiles are cloud-specific.
You use [networks](/Infrastructure/Resources/Networks/) and network profiles in vRealize Automation Cloud to help define the behavior of network provisioning for your [deployments](/Deployments/)

{{< img src="/Infrastructure/Configure/Network-Profiles/networkprofile-list.png" alt="Network Profiles" >}}

Network profile capability [tags](/Infrastructure/Configure/Tags/) are matched with constraint [tags](/Infrastructure/Configure/Tags/) in [cloud templates](/Design/Cloud_Templates/) to help control network selection.
Think of a network profile as a collection of workload-specific network characteristics.
A network profile contains specific information for a named [cloud account](/Infrastructure/Connections/Cloud-Accounts/) type and region in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) .

Learn more about Network Profiles and their capbilities:

1. [Learn more about network profiles in vRealize Automation Cloud](https://docs.vmware.com/en/VMware-Cloud-Assembly/services/Using-and-Managing/GUID-01E442EE-4004-4ED1-AA32-9CF73F24CB09.html)
2. [Network Automation with Cloud Assembly and NSX – part 1](https://blogs.vmware.com/management/2019/04/network-automation-cloud-assembly-and-nsx-part-1.html)

