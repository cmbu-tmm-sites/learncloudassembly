---
title: "Resource Flags"
weight: 15
---

Resource flag settings aren't part of the resource object properties schema. For a given resource, you add the flag settings outside of the properties section.

For example if we set the <strong>"dependsOnPreviousInstances:true"</strong> resource flag,  it creates a cluster resources sequentially. The default is false, which simultaneously creates all resources in a cluster, this is particularly useful for database clusters where primary and secondary nodes must be created, but secondary node creation needs configuration settings that connect the node to an existing, primary node.

or if in the other hand, we define the <strong>“preventDelete: true”</strong> resource flag, it protects a created resource from accidental deletion during updates, however If a user deletes the deployment, the resource is deleted. 

{{< img src="/Learn-in-5/Top-10-Cloud-Templates-features/Resource-Flags/Resource_Flags.png" alt="Resource Flags Example" >}}

Check out the [whole set of Resource Flags available in vRealize Automation](https://docs.vmware.com/en/vRealize-Automation/services/Using-and-Managing-Cloud-Assembly/GUID-B76918AE-D18D-4821-B160-F0CFAE173359.html) and/or see some of this properties in action at this short demo

Try it out in your lab or [vRealize Automation Cloud Trial](https://www.vmware.com/products/vrealize-automation.html)

Where to go from here - Learn more about [Cloud Assembly Tutorials](https://docs.vmware.com/en/vRealize-Automation/services/Using-and-Managing-Cloud-Assembly/GUID-DB7DC86A-8936-411D-B586-0724171FFB40.html), explore the [Top 10 Cloud Templates features](/Learn-in-5/Top-10-Cloud-Templates-features/)  and more.


