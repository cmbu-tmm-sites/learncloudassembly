---
title: "Pricing Cards"
weight: 80
---

A [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) pricing cards help cloud administrators define and assign the pricing policy for the monetary impact of your individual deployments to help you manage resources.

{{< hint info >}}For pricing to work on multi-tenant environments, you must have a separate vROPs instance for each vRA tenant.{{< /hint >}}

The pricing policy can then be assigned to specific projects to define a total price. The scope of all pricing cards could be set for Projects or Cloud Zones.
If Cost is selected, factors need to be provided which will be applied on the calculated cost.
If Rate is selected, absolute values need to be provided which will determine the price. 

New policies, assignments, and upfront pricing are priced during the next occurring data collection cycle.

{{< img src="/Infrastructure/Configure/Pricing-Cards/pricingcards-card.png" alt="Pricing Card Details" >}}

{{< hint info >}}If you change the All pricing cards are applied to setting, all existing pricing card assignments are deleted. Also, if the vRealize Operations endpoint is deleted from Cloud Assembly, all pricing cards and assignments are also deleted.{{< /hint >}}

More information for [How to use Pricing Cards](https://docs.vmware.com/en/vRealize-Automation/8.4/Using-and-Managing-Cloud-Assembly/GUID-376DBE2D-CDC1-4D90-8A6E-C0CCC61621B7.html?hWord=N4IghgNiBcIA4CcCWBjApgAhWBATAziAL5A)


