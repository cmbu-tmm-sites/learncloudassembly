---
title: "Tenant Management"
weight: 85
---

The <strong>Tenant Management</strong> 
[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) enables customer IT providers, to set up multiple tenants, or organizations, within each deployment. Providers can set up multiple tenant organizations and allocate infrastructure within each deployment. Providers can also manage users for tenants. Each tenant manages its own projects, resources, and deployments.

In a [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) multi-organization configuration, providers can create multiple organizations, and each tenant organization uses its own projects, resources and deployments. While providers cannot manage tenant infrastructure remotely, they can log in to tenants and manage infrastructure within their tenants
 
{{< img src="/Tenant-Management/tenantmanagement-top.png" alt="Tenant Management View" >}}

Multi-tenancy relies on coordination and configuration of three different VMware products as outlined below:

[Workspace ONE Access](https://docs.vmware.com/en/VMware-Workspace-ONE-Access/index.html) - This product provides the infrastructure support for multi-tenancy and the Active Directory domain connections that provide user and group management within tenant organizations.<br>

[vRealize Suite Lifecycle Manager](https://docs.vmware.com/en/VMware-vRealize-Suite-Lifecycle-Manager/index.html) - This product supports the creation and configuration of tenants for supported products. In addition, it provides some certificate management capabilities.<br>

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) - Providers and users log in to vRealize Automation to access tenants in which they create and manage deployments.