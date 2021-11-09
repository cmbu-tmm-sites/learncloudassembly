---
title: "Custom Names"
weight: 20
---
 
 <SPAN STYLE="font-size:18.0pt">
 <p style="color:#FF0000";>This option needs to be enabled - Contact your VMware Representative.</p>
 </SPAN>

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) 8.6.1 and Cloud Nov 2021 release, it was introduced the <b>custom naming</b> feature provides options for the customer to name the different [resource types](/Infrastructure/Resources/) like VMs, disks, networks, etc as per the custom template.

Here you can manage your <b>custom name templates</b> to be used for [resource types](/Infrastructure/Resources/) in the organization or [projects](/Infrastructure/Administration/Projects/).

{{< img src="/Infrastructure/Administration/Custom-Names/customnames-view.png" alt="Custom Names" >}}

You can create new <b>custom name templates</b> shared for the Organization or assigned to specific [projects](/Infrastructure/Administration/Projects/).

<b>Organization</b>: Create a default naming template that is applied to all deployments that do not have a project-level naming template.You cannot create more than one organization template. If the organization scope is not available, one already exists.

<b>Projects</b>: Create a naming template specific to the assigned projects. If both an organization and a project template exist, the project naming template takes precedence over the organization template.

You can also add naming templates for your different [resource types](/Infrastructure/Resources/).
Enter the properties and strings that you want generated as the resource name. Names must be unique. To ensure uniqueness, you must add the number generator to the the template. The number must be at the beginning or the end of the template, not in the middle.

For example, a compute resource type template might be <b>VM-${project.name}-${endpoint.endpointType}-${######}</b>

{{< img src="/Infrastructure/Administration/Custom-Names/customnames-template.png" alt="Custom Name Template" >}}

If you do not define naming templates for all [resource types](/Infrastructure/Resources/), the undefined [resource types](/Infrastructure/Resources/) default to the organization template. If an organization template does not exist, the undefined [resource types](/Infrastructure/Resources/) default to the system naming.

Please note that <b>Custom Naming</b> option under [Projects](/Infrastructure/Administration/Projects/) is also modified whenever this feature is enabled.

{{< img src="/Infrastructure/Administration/Custom-Names/customnames-project.png" alt="Custom Name Project" >}}