### Introduction


** Node-Exporter**

The node exporter can read system-level statistics about bare-metal nodes or virtual machines and export them for Prometheus. Using a DaemonSet, Kubernetes can run one node exporter per cluster node, and expose the node exporter as a service.


**BITNAMI NODE EXPORTER CONTAINER HELM CHARTS**
Deploying Bitnami applications as Helm Charts is the easiest way to get started with our applications on Kubernetes. Our application containers are designed to work well together, are extensively documented, and like our other application formats, our containers are continuously updated when new versions are made available.

 Try, test and work with the application in your local environment
 Deploy production-ready applications in your Kubernetes cluster.


**Why use Bitnami Helm Charts?**

Deploying Bitnami applications as Helm Charts is the easiest way to get started with our applications on Kubernetes. Bitnami ensures that the Helm Charts are always secure, up-to-date, and packaged using industry best practices. Bitnami is able to do this due to the monitoring and packaging automation that we have built throughout the years. When any vulnerability or updates arise for the application, we publish new container images and updated version tags for you to use.

This chart bootstraps Node Exporter on Kubernetes using the Helm package manager.

Bitnami charts can be used with Kubeapps for deployment and management of Helm Charts in clusters.


**Prerequisites**

You must install the IBM Cloud Block Storage plug-in from the catalog before you install this Chart. The Block Storage plug-in is a persistent, high-performance iSCSI storage that you can add to your apps by using Kubernetes Persistent Volumes (PVs).
Kubernetes 1.12+
Helm 3.0-beta3+


**What changes were introduced in this major version?**

Previous versions of this Helm Chart use apiVersion: v1 (installable by both Helm 2 and 3), this Helm Chart was updated to apiVersion: v2 (installable by Helm 3 only). Here you can find more information about the apiVersion field.
The different fields present in the Chart.yaml file has been ordered alphabetically in a homogeneous way for all the Bitnami Helm Charts.


**What you will get to know in this tutorial**

1-What is Bitnami Node Exporter Container Helm Charts

2-How to install and configure Node-exporter helm chart from bitnami

3-How to Upgarde to a new version.

