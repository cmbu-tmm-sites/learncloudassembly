---
title: "Deployments"
weight: 100
---

You can access the current status of your provisioned resources.<br> 

{{< img src="/Deployments/Deployments/deployment-single.png" alt="Deployment View" >}}

You can access detailed information for the deployment, such as: who owns the deployment, requested it, which Cloud Template has been used, expiration, created on and last updated dates. Additionally, Day 2 operations that affects all the resources within the deployment:

 <ul>
    <li><strong>Change Lease</strong></li>
    <li><strong>Change Owner</strong></li>
    <li><strong>Delete</strong></li>
    <li><strong>Edit Tags</strong></li>
    <li><strong>Power Off</strong></li>
    <li><strong>Update</strong></li>
    <li><strong>Change Project</strong></li>
    <li><strong>Power On</strong></li>
 </ul>

The Deployment view allows you to see a visual representation of the deployment <strong>Topology</strong>, which includes also access to the resources assoicated properties. You can use the Topology tab to understand the deployment structure and resources.

{{< img src="/Deployments/Deployments/deployment-details.png" alt="Deployment Full Detailed View" >}}

<strong>History</strong> Tab includes all the provisioning events and any events related to actions that you run after requested item is deployed. If there are any problems with the provisioning process, the History tab events will help you with troubleshoot the failures.

{{< img src="/Deployments/Deployments/deployment-history.png" alt="Deployment History" >}}

<strong>Price</strong> Tab displays pricing information is based on vRealize Operations Manager or CloudHealth integrations. You can use the pricing card to understand how much your deployment is costing your organization:

{{< img src="/Deployments/Deployments/deployment-priceoverall.png" alt="Deployment Price Analysis Overall" >}}

Price Analysis details are also available and visually represented:

{{< img src="/Deployments/Deployments/deployment-pricedetails.png" alt="Deployment Price Analysis Details" >}}

<strong>Monitor</strong> Tab data provides information about the health of your deployment based on data from vRealize Operations Manager:

{{< img src="/Deployments/Deployments/deployment-monitor.png" alt="Deployment Monitor" >}}

<strong>Alerts</strong> Tab provides active alerts on the deployment resources. You can dismiss the alert or add reference notes. The alerts are based on data from vRealize Operations Manager.:

{{< img src="/Deployments/Deployments/deployment-alerts.png" alt="Deployment Monitor" >}}

<strong>Optimize</strong> Tab provides utilization information about your deployment and offers suggestions for reclaiming or otherwise modifying the resources to optimize resource consumption. The optimization information is based on data from vRealize Operations Manager:

{{< img src="/Deployments/Deployments/deployment-optimize.png" alt="Deployment Rightsize & Underutilized Resources" >}}

<strong>Deployments Views: </strong>

You have two modes to display all your deployments: 
<strong>Card Wiew</strong>
{{< img src="/Deployments/Deployments/deployment-cardview.png" alt="Deployment Card View" >}}

<strong>Grid Wiew</strong>
{{< img src="/Deployments/Deployments/deployment-gridview.png" alt="Deployment Grid View" >}}

<strong>Deployments Search & Sorting Capabilities:</strong>

You can use search to locate deployments based on a broad range of values, not just the deployment name. 

{{< img src="/Deployments/Deployments/deployment-search.png" alt="Search Deployments with MOAD and S3 Strings" >}}

You can also locate deployments based on:

<ul>
    <li>Name, description, and who created the deployment</li>
    <li>Resource properties, such as resource name, IP address, image, region, tags, cloud account, or primary MAC address</li>
</ul>

When you use the search, observe the following advantages and constraints:

<ul>
    <li>The search is not case sensitive</li>
    <li>You can only search on initial strings, not embedded strings. For example, you can retrieve results for a network named <i>MyResourceName</i> using <i>My</i> or <i>MyResource</i>, but not ResourceName.</li>
    <li>You can search for values that might exist in more than one value type. For example, you can search deployments that contain a specific resource name and a specific tag. The search format must include a space between the values. The space is an implied <i>AND</i>. For example, you can search for MyResourceName <i>192.0.2.0</i></li>
</ul>

If you are looking for projects or resource types, use the filter rather than the search. You can also use the filters with the search to locate deployments.

{{< img src="/Deployments/Deployments/deployment-filter.png" alt="Filtering by Cloud Account and Sorting by creation." >}}

You also have the ability to <strong>Sort</strong> your deployment list by multiple criteria such as:

<ul>
    <li>Name (ascending)</li>
    <li>Name (descending)</li>
    <li>Price (ascending)</li>
    <li>Price (descending)</li>
    <li>Created on (ascending)</li>
    <li>Created on (descending)</li>
    <li>Expires on (ascending)</li>
    <li>Expires on (descending)</li>
    <li>Last updated (ascending)</li>
    <li>Last updated (descending)</li>
</ul>

{{< img src="/Deployments/Deployments/deployment-sort.png" alt="Sorting Expires on (descending)" >}}

