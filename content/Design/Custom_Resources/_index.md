---
title: "Custom Resources"
weight: 40
---

You can create custom resources, add them to the design canvas, and create [cloud templates](/Design/Cloud_Templates/) that support your design and deployment needs. 

Use [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) to create custom resources

Each custom resource is based on a [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) SDK inventory type and is created by a [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) workflow that has an output which is an instance of your desired SDK type. Primitive types, such as Properties, Date, string, and number are not supported for the creation of custom resources. 

<strong>Building Custom Resources</strong>

In order to build Custom Resources we will first need to build or identify a [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) workflow for our use case. You will need to have at least two [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) Workflows identified, one for the creation of the resource and one to destroy the resource when the [deployment](/Deployments/) is deleted. In this blog we will build out a simple use case of creating a vCenter Folder along with the machine [deployment](/Deployments/).

The [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) Workflow we will use in this example is called “Create Virtual Machine Folder” and the workflow to destroy the folder when the deployment is deleted is called “Delete Virtual Machine Folder”. Both of these are built in [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) Workflows.

{{< img src="/Design/Custom_Resources/customresourcecreatefolderwf.png" alt="Custom Resource Create Folder" >}}

{{< img src="/Design/Custom_Resources/customresourcedeletefolderwf-768x133.png" alt="Custom Resource Delete Folder" >}}

Notice that the “Create Virtual Machine Folder” has an Output for type VC:VmFolder, and the delete workflow has an Input for <i>VC:VmFolder</i>. This is needed in the event of a delete action.

Once we have identified the vRO workflow, we can then use that workflow in our Custom Resource object within [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly. Within Cloud Assembly you will see a [Design](/Design/) tab at the top, this is where you will configure [cloud templates](/Design/Cloud_Templates/) and custom resources. Click on Custom Resources and then New Custom Resource. Fill out the form with the following information:

<b>Name</b> – provide a name of the resource

<b>Description</b> – optional description

<b>Resource Type</b> – enter a name you want to give the resource, this will show up in the YAML code property – type. For example I entered Custom.CreateFolder.

<b>Activate</b> – choose this if you want the resource to be available now

<b>Scope</b> – define which projects can consume this resource, if you want all projects to see this resource then just leave it to the default.

After configuring the items above, you can then add the workflows you want to use under the <b>LifeCycle Actions</b> section. There are three types of actions you can configure – <i>Create</i>, <i>Update</i> and <i>Destroy</i>. The only two that are required are Create and Destroy. Notice that when you choose the “Create” workflow the system will auto-populate the External Type for you, in this case it found <i>VC:VmFolder</i>. This is an update we recently made to the product. This External Type is important in order for Update and Delete workflows to know what to do when they are triggered.

{{< hint info >}} Note: For vRealize Automation 8.0 and 8.1 customers, you will need to type or enter in the External Type manually. Make sure you choose the appropriate external type from the vRO Workflow. There should be a corresponding output and input between Create and Destroy workflows.{{< /hint >}}

{{< img src="/Design/Custom_Resources/mainsetuppage.png" alt="Main Set up Page" >}}

Another change that was recently made was putting the schema properties onto a Properties page. The schema elements are what get translated onto the [cloud templates](/Design/Cloud_Templates/) for configuration once the Custom Resource is dragged onto the [cloud templates](/Design/Cloud_Templates/) canvas.

{{< img src="/Design/Custom_Resources/propertiesschemepage.png" alt="Properties Scheme" >}}

Once you create the Custom Resource it will show up in the [cloud templates](/Design/Cloud_Templates/) as a Resource Type on the left hand side. 
{{< hint info >}} Note: If you modified the scope of the Custom Resource to a certain Project, then the Custom Resource will only show up if this [cloud templates](/Design/Cloud_Templates/) is also tied to the same Project.{{< /hint >}}

{{< img src="/Design/Custom_Resources/customresourceblueprintcanvas-1024x550.png" alt="Custom Resource Design Canvas" >}}

Once you drag the Custom Resource onto the canvas then the [cloud templates](/Design/Cloud_Templates/) YAML code will reflect the object. In this example I have already filled out the needed input bindings and path to the proper [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) inventory section for <i>VC:Folders</i>. With this workflow we have both an Input for the folder name (type: string) and an object to query the parent folder (type: object). When you want to query via type:object then you will need to list out the relevant [vRealize Orchestrator](https://www.vmware.com/products/vrealize-orchestrator.html) inventory path, in this case it is <i>$data: ‘vro/data/inventory/VC:VmFolder’</i>.

{{< img src="/Design/Custom_Resources/customresourceyamlfolder.png" alt="Custom Resource YAML Construct" >}}

You can now deploy the [cloud templates](/Design/Cloud_Templates/) from Cloud Assembly or Service Broker.. Once deployed you can see some information about the Custom Resource in the [deployment](/Deployments/)screen.

{{< img src="/Design/Custom_Resources/customresourcedeployed.png" alt="Custom Resource Deployed" >}}

You can also add Day-2 Action workflows to the Custom Resource. From the Custom Resource page go to the bottom of the page and you will see Additional Actions section.

{{< img src="/Design/Custom_Resources/addtionalactionssetup-768x138.png" alt="Additional Actions" >}}

These actions will present themselves in the Action dropdown when you select the custom resource from the Deployment Topology.

{{< img src="/Design/Custom_Resources/renameactionforfolder-768x347.png" alt="Rename Action Folder" >}}