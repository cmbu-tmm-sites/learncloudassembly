---
title: "Projects"
weight: 10
---

You create a project to which you add members and [cloud zones](/Infrastructure/Configure/Cloud-Zones/) so that the project members can deploy their [cloud templates](/Design/Cloud_Templates/) to the associated zones.

As the [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly administrator, you create a project for a development team. You can then assign a project administrator or you can operate as the project administrator.

{{< img src="/Infrastructure/Administration/Projects/projects-top.png" alt="Projects List" >}}

When you create a <strong> new Project </strong>, you need to 

1. Give it a name.
After the project is created and configure, you will be able to see an Overview of the resources that belong to the project.

{{< img src="/Infrastructure/Administration/Projects/projects-summary.png" alt="Projects Summary" >}}

2. Click the Users tab.
To make deployments by project members accessible only to the requesting user, turn off Deployment sharing. To ensure that you can assign the ownership of a deployment to another member of the project, verify that the Deployment sharing is turned on. Add users with assigned roles.

{{< img src="/Infrastructure/Administration/Projects/projects-users.png" alt="Project Users and Roles " >}}

3. Click the Provisioning tab and add one or more [cloud zones](/Infrastructure/Configure/Cloud-Zones/).
Add any [cloud zones](/Infrastructure/Configure/Cloud-Zones/). and [virtual private zones](/Infrastructure/Configure/Virtual-Private-Zones/) that contain the resources that support the [cloud templates](/Design/Cloud_Templates/) deployed by the project users.

For each zone, you can set a zone priority and you can limit the amount of resources that the project can use. The possible limits include the number of instances, memory, and CPUs. For vSphere cloud zones only, you can configure storage limits for deployed resources that are based on vSphere VM templates. The storage limits are evaluated with you request deployment and when you make changes using the resize disk, resize boot disk, remove disk, and the update count actions. These storage limits do not apply to other resource types such as AWS, Microsoft Azure, or Google Cloud Platform.

As you add each zone and apply limits, don't limit the project resources so narrowly that the members cannot deploy their [cloud templates](/Design/Cloud_Templates/).

When your users submit a deployment request, the zones are evaluated to determine which zones have the resources to support the deployment. If more than one zone supports the deployment, then the priority is evaluated and the workload is placed on the one with the higher priority, which is the lowest integer.

{{< img src="/Infrastructure/Administration/Projects/projects-provisioning.png" alt="Project Provisioning Cloud Zones " >}}

Additionally you can define at a project level:

<i>Resource Tags</i>: Specify the tags to be applied to machines provisioned in this project.<br> 
<i>Constraints</i>: Specify constraints that should be applied to all requests in this project. <br>
<i>Custom Properties</i>: Specify the custom properties that should be added to all requests in this project.
<i>Custom Naming</i>: Specify the naming template to be used for machines, networks, security groups and disks provisioned in this project. <br>
<i>Request Timeout</i>: If this project team is deploying [cloud templates](/Design/Cloud_Templates/)  that need more than 2 hours to provision, you can specify an extended period before the deployment fails. If both the [cloud templates](/Design/Cloud_Templates/)  and the project include timeout values, the largest value takes precedence.<br>
<i>Cloud Zone Mapping for [cloud templates](/Design/Cloud_Templates/)  Terraform Resources</i>: Allow Terraform resources to deploy to [cloud zones](/Infrastructure/Configure/Cloud-Zones/) in this project.<br>

{{< img src="/Infrastructure/Administration/Projects/projects-settings.png" alt="Project Provisioning Settings " >}}

4. Specify the [kubernetes zones](/Infrastructure/Configure/Kubernetes-Zones/) that can be used in this project for provisioning of clusters. 

{{< img src="/Infrastructure/Administration/Projects/projects-k8zones.png" alt="Kubernetes Zones " >}}

5. Click Create.

After Creating a project, you have access to the Integration Tab, which exposes the Version Control  Servers and Repositories used in the project for [cloud templates](/Design/Cloud_Templates/) and Terraform Configuration Files.

{{< img src="/Infrastructure/Administration/Projects/projects-integrations.png" alt="Version Control Integrations " >}}

<strong>Test Configuration</strong><br>
This option validate your configurations, by executing simulated provisioning requests. Based on the provided values, the requests will go through the projects, [cloud zones](/Infrastructure/Configure/Cloud-Zones/) and profiles configurations, however will not make actual provisionings to the [cloud account](/Infrastructure/Connections/Cloud-Accounts/).

{{< img src="/Infrastructure/Administration/Projects/projects-test-configuration.png" alt="Test Configuration" >}}