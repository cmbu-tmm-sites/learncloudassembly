---
title: "Custom Roles"
weight: 75
---

Custom roles can be assigned to [users and groups](/Infrastructure/Administration/Users-and-Groups/) in addition to their already existing service roles to provide an extra set of permissions.

These permissions apply across an Organization.  Users can be extended view and manage permissions over specific portions of Cloud Assembly, Service Broker, and CodeStream currently.  You can read more about custom user roles in the [product documentation](https://docs.vmware.com/en/vRealize-Automation/8.4/Using-and-Managing-Cloud-Assembly/GUID-6083A7EE-72F7-44E0-ACF4-87B4CF197842.html).  

Examining the screenshot, granular permissions can be assigned for Approvals, Infrastructure, Policies, XaaS actions and resources, and (not shown) Pipelines.  In the example, I will be giving Vincent the ability to Manage Approvals across the Organization.  Multiple permissions can be selected for a role.  The first step is to create the role.

{{< img src="/Infrastructure/Administration/Custom-Roles/customroles-view.png" alt="New Custom Role " >}}

Once the role is created, I can assign a role to users or groups.  Before making an assignment, users and groups are defined in Identity and Access Management with rights to the services they would view or manage.  If that’s already done, type the username or group name in the search field then select the desired results and click Add.

{{< img src="/Infrastructure/Administration/Custom-Roles/customroles-assign.png" alt="New Custom Role " >}}

At any time you can view all custom roles, assign additional users, and delete the role by selecting Custom Roles.  Clicking the role will open the permissions list and show what has been configured for that role; essentially the same view as we saw when creating the role.

{{< img src="/Infrastructure/Administration/Custom-Roles/customroles-list.png" alt="Custom Roles " >}}

If you want to view user assignments for a given role, you can select [Users and Groups](/Infrastructure/Administration/Users-and-Groups/). 