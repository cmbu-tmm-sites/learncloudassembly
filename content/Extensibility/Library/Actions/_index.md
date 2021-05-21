---
title: "Actions"
weight: 50
---

## Actions

<strong>Action Based Extensibility (ABX) Actions</strong> are small, lightweight scripts of code used to specify an action and how that action is to perform.

ABX Actions execute in Public Cloud via Function as a Service Lambda in AWS Azure Functions in Azure or inside [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) *please note that vRAC provides this capability by deploying the [Cloud Extensibility Proxy (CEXP)](https://blogs.vmware.com/management/2020/12/vro-vrac.html) *

{{< img src="/Extensibility/Library/Actions/abx-list.png" alt="ABX Actions Library" >}}

You can use the action editor to create custom scripts as well as define package dependencies and requirements for your extensibility ABX actions.
You can also import ABX extensibility actions from pre-defined vRealize Automation Cloud Assembly action templates or from a ZIP file. 

Here you can establish and release versions for ABX actions, select FaaS Provider, set custom limits and retry options and test ABX Actions Locally Executions.

ABX Actions supports Python 3 , PowerShell, NodeJS & JavaScript Languages Available. 

{{< img src="/Extensibility/Library/Actions/abx-editor.png" alt="ABX Editor" >}}

Action Constant or Secrents can be consumed as input values to your ABX extensibility actions.
Secrets are available for all FaaS providers and runtimes. 
Secrets use the <code>context.getSecret()</code> function to run as part of your script. This function uses the name of the secret as a parameter.

{{< img src="/Extensibility/Library/Actions/abx-secrets.png" alt="ABX Input Secrets" >}}



### Reference
 * [Cloud Management ABX Blogs](https://blogs.vmware.com/management/?s=ABX)
