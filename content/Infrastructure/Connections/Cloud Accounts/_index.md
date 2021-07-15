---
title: "Cloud Accounts"
weight: 10
---

## Cloud Account Types

Cloud accounts are the configured permissions that [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly uses to collect data from the regions or data centers, and to deploy [cloud templates](/Design/Cloud_Templates/) to those regions.
Resource information such as network and security, compute, storage, and tags content is data-collected from your cloud accounts.
The collected data includes the regions that you later associate with [cloud zones](/Infrastructure/Configure/Cloud-Zones/).

{{< img src="/Infrastructure/Connections/Cloud-Accounts/cloudaccounts-view.png" alt="Cloud Accounts Available " >}}

You can configure a [VMware Cloud Foundation (VCF)](https://www.vmware.com/products/cloud-foundation.html) as a cloud account within [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly to use workload domains.
As a cloud administrator, you can create a [VMware Cloud on AWS](https://www.vmware.com/products/vmc-on-aws.html) cloud account for account regions to which your team will deploy [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) cloud templates.

## VMware Cloud Foundation as a first-class cloud account

Support for VCF as an endpoint to provision [cloud templates](/Design/Cloud_Templates/) into a vSphere environment

1. Expose VCF as a unified entity 
2. Create a cloud accounts & cloud zones
3. Simplify the ongoing lifecycle management
4. Setup & configure cloud for full consumption

{{< img src="/Infrastructure/Connections/Cloud-Accounts/vcf-view.png" alt="Cloud Accounts - VCF " >}}
