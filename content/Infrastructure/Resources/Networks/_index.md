---
title: "Networks"
weight: 20
---

In [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html), cloud administrators can view and edit the network resources that have been data-collected from the [cloud accounts](/Infrastructure/Connections/Cloud-Accounts/) and integrations that are mapped to your project.

The [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly Networks page contains information such as:

1. Networks and load balancers that are defined externally in the network domain of your cloud account, for example in vCenter, NSX-T, or Amazon Web Services.
2. Networks and load balancers that have been deployed by the cloud administrator.
3. IP ranges and other network characteristics that have been defined or modified by your cloud administrator.
4. External IPAM provider IP ranges for a particular address space in an provider-specific external IPAM integration.

## Networks

You can view and edit networks and their characteristics, for example to add [tags](/Infrastructure/Configure/Tags/) or remove support for public IP access. You can also manage network settings such as DNS, CIDR, gateway, and [tag](/Infrastructure/Configure/Tags/)values. You can also define new, and manage existing, IP ranges within a network.

{{< img src="/Infrastructure/Resources/Networks/resourcesnetworks-view.png" alt="Networks Resources View " >}}

## IP Ranges

Use an IP range to define or make changes to the start and end IP address for a particular network in your organization. You can display and manage IP ranges for listed networks. If the network is managed by an external IPAM provider, you can manage IP ranges in connection with the associated IPAM integration point.

If you are using an external IPAM integration for a particular IPAM provider, you can use the <b>External IP range</b> to select an IP range from an available external IPAM integration point. This process is described within the context of an overall external IPAM integration workflow at [Configure a network and network profile to use external IPAM for an existing network in vRealize Automation](https://docs.vmware.com/en/vRealize-Automation/8.4/Using-and-Managing-Cloud-Assembly/GUID-9AE32BD7-2D1B-4FEE-881F-A0EDE5907D10.html).

{{< img src="/Infrastructure/Resources/Networks/resourcesipranges-view.png" alt="IP Ranges View " >}}

## IP Addresses

You can see the IP addresses that are currently used by your organization and display their status, for example available or allocated. The IP addresses that are displayed are either IP addresses that are managed internally by [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) or IP addresses that are designated for deployments that contain an external IPAM provider integration. External IPAM providers manage their own IP address allocation.

If the network is managed internally by [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html), and not by an external IPAM provider, you can also release IP addresses.

{{< img src="/Infrastructure/Resources/Networks/ipaddresses-view.png" alt="IP Addressess View " >}}

## Load Balancers

You can manage information about available load balancers for the account/region [cloud account](/Infrastructure/Connections/Cloud-Accounts/) in your organization. You can open and display the configured settings for each available load balancer. You can also add and remove tags for a load balancer.

{{< img src="/Infrastructure/Resources/Networks/loadbalancers-view.png" alt="Load Balancers View " >}}

## Network Domains

The network domains list contains related and non-overlapping networks.

{{< img src="/Infrastructure/Resources/Networks/networkdomains-view.png" alt="Network Domains View " >}}