---
title: "Storage"
weight: 40
---

A cloud administrator can work with storage resources and their capabilities, which are discovered through [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) data collection from associated [cloud accounts](/Infrastructure/Connections/Cloud-Accounts/).

Storage resource capabilities are exposed through [tags](/Infrastructure/Configure/Tags/) that typically originate at the source cloud account. A cloud administrator can choose to apply additional [tags](/Infrastructure/Configure/Tags/) directly to storage resources though, using vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly. The additional [tags](/Infrastructure/Configure/Tags/) might label a specific capability for matching purposes at provisioning time.

## Storage Policies

Storage policies that can be used for provisioning.

Select one or more defined storage policies to add or edit their [tag](/Infrastructure/Configure/Tags/) definitions. Use [tags](/Infrastructure/Configure/Tags/) to make specific storage capabilities, such as thin provisioning or Net App FlexClone, available for that policy.

{{< img src="/Infrastructure/Resources/Storage/resourcestoragepolicy-view.png" alt="Storage Policies View " >}}

## Datastores and datastore clusters

Datastores and datastore clusters that can be used for provisioning disks. 
You can add capability [tags](/Infrastructure/Configure/Tags/) to vSphere Datastores / Clusters. The [tags](/Infrastructure/Configure/Tags/) that you add can then be referred within a [Cloud Template](Design/Cloud_Templates/) to provide additional placement constraints for provisioning disks.

{{< img src="/Infrastructure/Resources/Storage/resourcedatastore-view.png" alt="Datastores and datastore clusters View " >}}

## Storage accounts

Storage accounts that can be used for provisioning.
Select one or more defined Microsoft Azure storage accounts to add or edit their [tag](/Infrastructure/Configure/Tags/) definitions. Use [tags](/Infrastructure/Configure/Tags/) to make specific storage capabilities, such as general purpose, BLOB, standard, or premium for the Microsoft Azure cloud account.

{{< img src="/Infrastructure/Resources/Storage/resourcestorageaccounts-view.png" alt="Storage accounts View " >}}