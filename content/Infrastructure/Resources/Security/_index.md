---
title: "Security"
weight: 30
---

After you add a [cloud account](/Infrastructure/Connections/Cloud-Accounts/) in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly, data collection discovers the [cloud account](/Infrastructure/Connections/Cloud-Accounts/)'s network and security information and makes that information available for use in [network profiles](/Infrastructure/Configure/Network-Profiles/) and other options.

Security groups and firewall rules support network isolation. Security groups are data-collected. Firewall rules are not data-collected.

You can view the available security groups and add or remove [tags](/Infrastructure/Configure/Tags/) for selected security groups. A [cloud template](/Design/Cloud_Templates/) author can assign one or more security groups to a machine NIC to control security for the deployment

Existing security groups are displayed and classified in the <b>Origin</b> column as <b>Discovered</b>. On-demand security groups that you create in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly, either in a cloud template or in a network profile, are displayed and classified in the b>Origin</b> column as <b>Managed by Cloud Assembly</b>.
 On-demand security groups that you create as part of a [network profile](/Infrastructure/Configure/Network-Profiles/) are internally classified as an isolation security group with pre-configured firewall rules and are not added to a [cloud template](/Design/Cloud_Templates/) design as a security group resource. On-demand security groups that you create in a [cloud template](/Design/Cloud_Templates/) design, and that can contain express firewall rules, are added as part of a security group resource that is classified as <b>new</b>.

Several filtering options are available.

{{< img src="/Infrastructure/Resources/Security/resourcessecurity-view.png" alt="Security Groups View " >}}
