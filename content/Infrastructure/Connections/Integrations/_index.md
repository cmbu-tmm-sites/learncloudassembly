---
title: "Integrations"
weight: 20
---

## Integrations enable you to add external systems to vRealize Automation

Integrations include [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html), configuration management and other external systems such as GitHub, Ansible, Puppet, and external IPAM providers such as Infoblox.
[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly supports integration with various flavors of Git repositories so that you can manage VMware [cloud templates](/Design/Cloud_Templates/) and action scripts under source control.

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) can work with [vRealize Operations Manager](https://www.vmware.com/products/vrealize-operations.html) to perform advanced workload placement, provide deployment health and virtual machine metrics, and display pricing.
You can configure a [SaltStack Config](https://www.vmware.com/products/vrealize-automation/saltstack-config.html) integration to access the [SaltStack Config](https://www.vmware.com/products/vrealize-automation/saltstack-config.html) service and use [SaltStack Config](https://www.vmware.com/products/vrealize-automation/saltstack-config.html) objects and [actions](/Extensibility/Library/Actions/) in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html).

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-view.png" alt="Cloud Integrations Available " >}}

<strong>Typical integrations for automation</strong>

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-typical.png" alt="Typical Integrations " >}}

<strong>vRealize Operations Manager</strong>

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) can work with [vRealize Operations Manager](https://www.vmware.com/products/vrealize-operations.html) to perform advanced workload placement, provide deployment health and virtual machine metrics, and display pricing.
Integration between the two products must be on-premises to on-premises, not a mix of on-premises and cloud.

 1. Advanced workload placement using vRealize Operations Manager
 2. Deployment monitoring based on vRealize Operations Manager
 3. Resource management and deployment optimization using vRealize Operations Manager metrics in vRealize Automation

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-vrops.png" alt="vROPs Integration " >}}

<strong>Ansible Tower Integration</strong>

Support for Ansible Tower allows customers to run Ansible Tower Job Templates from our blueprint canvas. 
Incorporating existing Ansible Tower instances into vRealize Automation gives customers another option for configuration management along with Puppet and Ansible Open Source. 

The Ansible Tower and/or Engine can be on-prem or in the cloud. The nodes that will be managed or deployed could also be on-prem or in the cloud. 
The integration provides maximum flexibility when integrating with these solutions.

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-ansible.png" alt="Ansible Integrations " >}}

<strong>Version Control | Git Integration</strong>

The [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) supports integration with Git repositories so that you can manage VMware cloud templates, Terraform Configurations and [actions](/Extensibility/Library/Actions/) Scripts under source control. This functionality facilitates auditing and accountability of processes around deployment.

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly supports different [flavors](/Infrastructure/Configure/Flavor-Mappings/) of Git integration as described in the following list. Each of these options is a separate integration.

1. GitHub cloud, GitHub Enterprise on-premises
2. GitLab cloud GitLab Enterprise on-premises
3. BitBucket on-premises

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-git.png" alt="Version Control Server Integrations " >}}

<strong>Active Directory Integration</strong>

Allow consumption of Cloud Zones based on Tags 
Dynamic validation of AD integration settings during authoring
Machine assigned to correct Organization unit based on the Project the deployment user is assigned in Cloud Assembly.
When deployment is deleted the machine account is Active Directory is also deleted.
vRA Cloud Requires deployment of new On-Prem Extensibility Action appliance

{{< img src="/Infrastructure/Connections/Integrations/cloudaintegrations-ad.png" alt="Active Directory Integration " >}}

<strong>External IPAM integration</strong>

You can create a provider-specific external IPAM integration point to manage the IP addresses used in your [cloud templates](/Design/Cloud_Templates/) deployments. When using an external IPAM integration point, IP addresses are obtained from and managed by the designated IPAM provider rather than from [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html).

You can create a provider-specific IPAM integration point to manage IP addresses and DNS settings for [cloud templates](/Design/Cloud_Templates/) deployments and VMs in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html).
