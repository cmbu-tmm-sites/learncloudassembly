---
title: "Cloud Templates"
weight: 20
---

The <strong>Cloud Templates</strong> tab will allow you to manage your Cloud Templates.<br> 
You will be able to access Cloud Templates metadata such as, <b>Source Control</b>, <b>Project</b>, <b>Last Updated</b>, <b>Updated By</b> and <b>Release Versions</b>.
More importantly, you can create, update, sync repos, clone, deploy, download or delete Cloud Templates.
Please note that you can filter by <b>Project</b> and/or <b>Property Group</b>.

{{< img src="/Design/Cloud_Templates/Cloud-Templates-Top.png" alt="Cloud Templates Default View" >}}

[vRealize Automation](https://www.vmware.com/products/vrealize-automation.html)Cloud Assembly creates and saves cloud templates as code, which allows you to easily design and reuse Cloud Templates.

You can build a Cloud Template from a blank canvas or take advantage of existing code.

You use the design page to create [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly template specifications for the machines or applications that you want to provision.

<strong>1. Locate resources.</strong><br>
<strong>2. Drag resources to the canvas.</strong><br>
<strong>3. Connect resources.</strong><br>
<strong>4. Configure resources by editing the cloud template code.</strong><br>

{{< img src="/Design/Cloud_Templates/Cloud-Templates-Design-Canvas.png" alt="Cloud Templates Design Canvas" >}}

From the design page, you can also change the cloud template name, version or revert to versions, clone, or deploy a template.

The code editor allows you to type, cut, copy, and paste code directly. If you're uncomfortable editing code, you can select a resource in the design canvas, click the code editor Properties tab, and enter values there. Property values that you enter appear in the code as if you had typed them directly.

{{< img src="/Design/Cloud_Templates/Cloud-Templates-Editor-Properties.png" alt="Cloud Templates Editor and Properties view" >}}

Note that you can copy and paste code from one cloud template to another.

<b>Cloud Template cloning</b>
To clone a template, go to Design, select a source, and click Clone. You clone a cloud template to create a copy based on the source, then assign the clone to a new project or use it as starter code for a new application.

<b>Uploading and downloading</b>
The [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly [Marketplace](/Marketplace/) offers finished cloud templates to jumpstart your effort. 

In addition, you can upload, download, and share cloud template YAML code in any way that makes sense for your site. You can even modify template code using external editors and development environments.

<b>Terraform</b>
You can also create cloud templates that include Terraform Configuration constructs.
Learn more in the [Terraform Service in vRA](https://blogs.vmware.com/management/2020/09/terraform-service-in-vra.html)