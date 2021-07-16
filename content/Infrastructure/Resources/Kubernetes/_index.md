---
title: "Kubernetes"
weight: 70
---

Cloud administrators can add, view, and manage the configuration of deployed Kubernetes clusters and namespaces, both generic and Pacific-based, in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly.

This page contains tabs for Clusters, Namespaces, Supervisor Clusters and Supervisor Namespaces. You can select one of these tabs to view and manage the analogous resources. Most typically, this page facilitates management of deployed clusters and namespaces.

## Cluster
 A cluster is a group of Kubernetes nodes distributed across one or more physical machines. This page shows provisioned and undeployed clusters that have been configured for use on your [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly instance. You can click on a cluster to view information about its current status. When you deploy a cluster, it includes a link to a <i>Kubconfig</i> file that is accessible only for cloud administrators. This file grants full admin privileges over the cluster including a list of namespaces.

 {{< img src="/Infrastructure/Resources/Kubernetes/resourceskubernetes-cluster.png" alt="Kubernetes Cluster " >}}

<strong>Supervisor clusters</strong> are unique to vSphere instances and use ESXI as their worker nodes instead of Linux.

## Namespaces
Namespaces are virtual clusters that provide administrators with a way to segregate cluster resources. They facilitate management of resources among large groups of users and organizations. As a form of role-based access control, a cloud administrator can enable users to add namespaces to a project when they request a deployment and then later manage those namespaces from the Kubernetes Clusters page. When you deploy a namespace, it includes a link to a kubeconfig file that enables valid users, such as developers, to view and manage some aspects of that namespace.

{{< img src="/Infrastructure/Resources/Kubernetes/resourceskubernetes-namespace.png" alt="Kubernetes Namespace " >}}

<strong>Supervisor clusters</strong> & <strong>supervisor namespaces</strong> exist only on vSphere instances and provide Kubernetes-like access to vSphere objects.

