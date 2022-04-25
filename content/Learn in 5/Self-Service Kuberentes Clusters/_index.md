---
title: "Enabling self-service Kubernetes clusters with Tanzu"
draft: true
---

## Setting up the infrastructure
Configuring the infrastructure is a one-time configuration to enable the on-demand deployment of Kubernetes clusters on vSphere.

### Prerequisites

- vSphere endpoint
  - Workload Management enable
  - Supervisor Cluster available

### Add a Supervisor Cluster
To bring a Supervisor Cluster under Cloud Assembly's management, it is added to the Kubernetes resources.

1) Click the ADD SUPERVISOR CLUSTER button
2) Select the vSphere endpoint from the menu
3) Select the Supervisor cluster from the menu
4) Click ADD

{{< img src="supervisor-cluster.png" alt="Add a Supervisor Cluster" >}}

### Create a Kubernetes Zone
A Kubernetes Zone ui

### Assign a Kubernetes Zone to a Project

## Enable on-demand Kubernetes clusters

Enabling on-demand Kubernetes clusters is a two-step process, firstly a Cloud Template is created to configure the request, which is then published to the content catalog with a (optional) custom form to help guide the end user.

### Create a Cloud Template

### Publish to Service Broker Catalog