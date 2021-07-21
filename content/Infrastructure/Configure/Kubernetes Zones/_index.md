---
title: "Kubernetes Zones"
weight: 30
---

Kubernetes zones enable cloud administrators to define policy-based placement of Kubernetes clusters and namespaces and supervisor namespaces used in [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html)  Cloud Assembly deployments.
 An administrator can use this page to specify what clusters are available for provisioning of [Kubernetes](/Infrastructure/Resources/Kubernetes/) namespaces and what properties are acceptable for clusters.

{{< img src="/Infrastructure/Configure/Kubernetes-Zones/kuberneteszone-display.png" alt="Kubernetes Zone List" >}}

You can create Kubernetes zones with supervisor namespaces on vSphere in the same way that you work with generic [Kubernetes](/Infrastructure/Resources/Kubernetes/) namespaces. To add a supervisor namespace to a Kubernetes zone, you must associate the zone with a vSphere 7 endpoint that contains the desired Pacific namespace resources

{{< img src="/Infrastructure/Configure/Kubernetes-Zones/kuberneteszone-supervisor.png" alt="Kubernetes Supervisor Cluster" >}}