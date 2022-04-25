---
title: "Deploy Tanzu CE AWS"
weight: 25
---

VMware [Tanzu Community Edition](https://tanzucommunityedition.io/) is a full-featured, easy-to-manage Kubernetes platform for learners and users, especially those working in small-scale or preproduction environments.

vRealize Automation's [cloud template](/Design/Cloud_Templates/) are iterative, declarative code objects that define the desired state of a deployed resource.

You can use the vRealize Automation's [Tanzu-CE-bootstrap](https://gitlab.com/moffzilla/tanzuce-bootstrap) Cloud Template with embedded [cloud-init](https://cloud-init.io/) + "[input parameters](https://docs.vmware.com/en/vRealize-Automation/services/Using-and-Managing-Cloud-Assembly/GUID-6BA1DA96-5C20-44BF-9C81-F8132B9B4872.html?hWord=N4IghgNiBcIJYDsAOBXALgZxAXyA)", for deploying a Tanzu CE cluster at AWS VMs, this way, you remove the complexity of the pre-requisites installation, settings configurations and automate the actual Tanzu CE cluster's creation at AWS, furthermore, you can include specific custom user selections at request time for different types of Tanzu CE installations configurations.

{{< img src="/Learn-in-5/Deploy-Tanzu-CE-AWS/tanzu_ce_ct.png" alt="Cloud Template with Cluster and Instance AWS RDS Resources" >}}

Try it out in your lab or [vRealize Automation Cloud Trial](https://www.vmware.com/products/vrealize-automation.html)<br>

Learn more about [Cloud Assembly Tutorials](https://docs.vmware.com/en/vRealize-Automation/services/Using-and-Managing-Cloud-Assembly/GUID-DB7DC86A-8936-411D-B586-0724171FFB40.html), [What can I do if a Cloud Assembly deployment fails](https://docs.vmware.com/en/vRealize-Automation/services/Using-and-Managing-Cloud-Assembly/GUID-970CA971-65B7-4747-BF35-A54C1C0B849B.html) and more

Where to go from here - [Get Started with VMware Cloud on AWS](https://www.vmware.com/products/vmc-on-aws/get-started.html??src=ps_622b0c40e1e21&cid=7012H000001lI5H&gclid=CjwKCAjw0a-SBhBkEiwApljU0rgQijDsy5zuVU1DvGbH80auGejS-3CINy58fK0SpvRxHwzbfVVw7RoC2n8QAvD_BwE&gclsrc=aw.ds), learn about [Low-Cost Migrations to VMWare Cloud on AWS with vRealize Cloud Management](https://blogs.vmware.com/management/2021/06/low-cost-migrations-to-vmware-cloud-on-aws-with-vrealize.html) and [vRealize Automation & VMware Solution Self-Service Hybrid Cloud Hyperscalers](https://blogs.vmware.com/management/2021/05/vra-hyperscalers.html).


