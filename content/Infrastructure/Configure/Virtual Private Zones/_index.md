---
title: "Virtual Private Zones"
weight: 20
---

Centralized management of tenant infrastructure
1. Virtual Private Zones (VPZ)
2. Provider can allocate that VPZ into a different tenant organization
Shared and dedicated [infrastructure multi-tenancy](/Tenant-Management/)

{{< img src="/Infrastructure/Configure/Virtual-Private-Zones/virtualcloudzones-view.png" alt="Virtual Cloud Zones View" >}}

Provider administrators have the ability to share infrastructure by creating and assigning Virtual Private Zones to Tenant Organizations.  VPZs can be used in a single tenant Organization as well. 

{{< img src="/Infrastructure/Configure/Virtual-Private-Zones/virtualcloudzones-list.png" alt=" Virtual Cloud Zones List" >}}

Once the VPZ is allocated to a Tenant, the Tenant Administrator has the ability to add a VPZ to Projects within their assigned Tenant. 
At this point, the VPZ behaves in a similar manner to a Cloud Zone.  You can even set resource limits just as you would with Cloud Zones.
The new configuration options allow the Provider Admin to assign Images and Flavors to a single Tenant or all Tenants.  
Tenant admins can then use those constructs within their Tenants for deployments.  
The setup of Images and Flavors within Tenant Management, mirrors the setup of the Images and Flavors under Infrastructure in vRA. 

{{< img src="/Infrastructure/Configure/Virtual-Private-Zones/virtualcloudzones-assignment.png" alt="Virtual Cloud Zones assignment" >}}