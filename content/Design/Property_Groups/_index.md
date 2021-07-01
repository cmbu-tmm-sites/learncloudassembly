---
title: "Property Groups"
weight: 30
---

## Content

You can quickly add a property group to different vRealize Automation Cloud Assembly designs, which saves the time of adding the same multiple properties one by one. In addition, you have a single place to maintain or modify the set of properties, which ensures their consistent application.

{{< img src="/Design/Property_Groups/Property_Groups-list.png" alt="Property Groups List" >}}

here are two types of property groups.

<strong>Input property groups</strong> gather and apply a consistent set of properties at user request time. Input property groups can include entries for the user to add or select, or they might include read-only values that are needed by the design.

Properties for the user to edit or select can be readable or encrypted. Read-only properties appear on the request form but can't be edited. If you want read-only values to remain totally hidden, use a constant property group instead.

[How to create and use an input property group in vRealize Automation Cloud Assembly](https://docs.vmware.com/en/vRealize-Automation/8.4/Using-and-Managing-Cloud-Assembly/GUID-4D84F583-7E1A-4FA7-82D3-7DF0689736DD.html)

<strong>Constant property groups</strong> silently apply known properties. In effect, constant property groups are invisible metadata. They provide values to your vRealize Automation Cloud Assembly designs in a way that prevents a requesting user from reading those values or even knowing that they're present. Examples might include license keys or domain account credentials.

[How to create and use a constant property group in vRealize Automation Cloud Assembly](https://docs.vmware.com/en/vRealize-Automation/8.4/Using-and-Managing-Cloud-Assembly/GUID-E035224B-C725-4F93-96B0-BCA6C2E7AFBD.html)

<strong>Modifying a property group</strong>

Changes to a [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly property group affect every [cloud templates](/Design/Cloud_Templates/) that uses it, including ones that might have already been released to the Service Broker catalog.

The property group list and property group editing pages show the number of [cloud templates](/Design/Cloud_Templates/) that include the property group. To see which [cloud templates](/Design/Cloud_Templates/) would be affected by a change, click the number.

{{< img src="/Design/Property_Groups/Property_Groups-modify.png" alt="Property Groups Modifying" >}}

Before modifying a property group, make sure that the change is acceptable to everyone who is creating or updating [deployments](/Deployments/) based on the [cloud templates](/Design/Cloud_Templates/) listed.

<strong>Deleting a property group</strong>

Deleting a property group would cause errors in every [cloud templates](/Design/Cloud_Templates/) that uses it.

You cannot delete a property group until you manually remove it from all of the [cloud templates](/Design/Cloud_Templates/) in which it is included. To remove a property group from a [cloud templates](/Design/Cloud_Templates/), open the [cloud templates](/Design/Cloud_Templates/) in the design canvas.

You can learn more about Property Groups in the following Blogs:<br>
[ntroducing vRealize Automation Property Groups](https://blogs.vmware.com/management/2020/12/introducing-vrealize-automation-property-groups.html)<br>
[vRealize Automation Property Groups Enhancements](https://blogs.vmware.com/management/2021/06/vra-latest-property-groups-enhancements.html)