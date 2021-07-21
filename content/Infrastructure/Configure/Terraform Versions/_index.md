---
title: "Terraform Versions"
weight: 90
---

You can embed Terraform configurations as a resource in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) in Cloud Assembly.

{{< img src="/Infrastructure/Configure/Terraform-Versions/terraformservice.png" alt="Terraform Service" >}}

{{< img src="/Infrastructure/Configure/Terraform-Versions/terraformservice-details.png" alt="Terraform Service Description" >}}

Before you add a Terraform configuration to a [cloud template](/Design/Cloud_Templates/), set up and integrate your version control repository under [integrations](/Infrastructure/Connections/Integrations/).
With your repository and Terraform configuration files in place, you can design a Cloud Assembly template for them.

## Enable Terraform runtime versions
You can define the Terraform runtime versions available to users when deploying Terraform configurations. Note that Terraform configurations might also include internally coded version constraints.

{{< img src="/Infrastructure/Configure/Terraform-Versions/terraformservice-versions.png" alt="Terraform runtime versions" >}}

{{< hint info >}}For [vRealize Automation 8.X or on-prem](https://www.vmware.com/products/vrealize-automation.html) the Terraform Run Time defines a Kubernetes Namespace integration point for executing the Terraform Jobs, you have two options,  Managed Kubernetes cluster or External Kubeconfig{{< /hint >}}

For learning how to set up from scratch and test it, you can follow this blog: [Terraform Service in vRA Cloud Templates ](https://blogs.vmware.com/management/2020/09/terraform-service-in-vra.html)

You can find more examples here:  [vRealize Automation & Terraform OpenSource : Practical Examples - Part 5](https://blogs.vmware.com/management/2020/10/vra-terraform.html)

You can also [get started with the vRealize Automation Terraform Provider](https://blogs.vmware.com/management/2020/01/getting-started-with-vra-terraform-provider.html)