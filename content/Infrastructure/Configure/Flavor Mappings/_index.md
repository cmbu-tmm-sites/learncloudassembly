---
title: "Flavor Mappings"
weight: 40
---

A [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) flavor map is where you use natural language to define target deployment sizes for a specific [cloud account](/Infrastructure/Connections/Cloud-Accounts/)/region.

{{< img src="/Infrastructure/Configure/Flavor-Mappings/flavormapping-concept.png" alt="Flavors mapping to instance types in native clouds" >}}

Flavor maps express the deployment sizes that make sense for your environment. One example might be small for 1 CPU and 2 GB memory and large for 2 CPUs and 8 GB memory for a vCenter account in a named data center and t2.nano for an Amazon Web Services account in a named region.

{{< img src="/Infrastructure/Configure/Flavor-Mappings/flavormapping-display.png" alt="Flavor Mapping List" >}}


A flavor mapping associates a defined [cloud account](/Infrastructure/Connections/Cloud-Accounts/)/region with one or more data-collected sizing options or instance types. For example, a flavor of small might equate to a specific number of CPUs, allowing you to scale your [resources](/Infrastructure/Resources/) to the requirements of your target workload. 
Flavor mappings are regional settings.

{{< img src="/Infrastructure/Configure/Flavor-Mappings/flavormapping-details.png" alt="Flavor Mapping Details" >}}