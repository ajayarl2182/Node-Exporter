### Introduction

** Node-Exporter**

### **Install The Node Exporter Chart
** 
To start using any Bitnami Helm chart, it is necessary to add the Bitnami Helm charts repository to Helm and run the helm install command to deploy this chart. Follow these steps:

Add the Bitnami repository to Helm with the following command:

helm repo add bitnami **https://charts.bitnami.com/bitnami**

A Helm chart describes a specific version of a solution, also known as a “release”. The “release” includes files with Kubernetes-needed resources and files that describe the installation, configuration, usage and license of a chart.

Check that your Kubernetes cluster is running by executing the following command:

kubectl cluster-info

**Install Node Exporter by running the following:**

**NOTE: **
Remember that MY-RELEASE is a placeholder, replace it with the name you want to give to the chart or add the --generate-name to give the chart a random name.

helm install MY-RELEASE bitnami/node-exporter


**Node Exporter**

 Node Exporter s a Prometheus exporter for hardware and OS metrics exposed by *NIX kernels, written in Go with pluggable metric collectors.

**TL;DR**

helm repo add bitnami https://charts.bitnami.com/bitnami
helm install my-release bitnami/node-exporter

**Introduction**

This chart bootstraps Node Exporter on Kubernetes using the Helm package manager.
Bitnami charts can be used with Kubeapps for deployment and management of Helm Charts in clusters.

**Prerequisites**

* Kubernetes 1.12+
* Helm 3.0-beta3+

**Installing the Chart**

**Add the bitnami charts repo to Helm:**

helm repo add bitnami https://charts.bitnami.com/bitnami

**To install the chart with the release name my-release:**

helm install my-release bitnami/node-exporter

The command deploys Node Exporter on the Kubernetes cluster in the default configuration. The configuration section lists the parameters that can be configured during installation.

**Uninstalling the Chart**

To uninstall/delete the my-release release:

helm delete my-release

The command removes all the Kubernetes components associated with the chart and deletes the release.

**Parameters**

Specify each parameter using the --set key=value[,key=value] argument to helm install. For example the following command sets the minReadySeconds of the Node Exporter Pods to 120 seconds.

 **Run this Command**

helm install my-release --set minReadySeconds=120 bitnami/node-exporter

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

**Run this Command**

helm install my-release -f values.yaml bitnami/node-exporter

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. 

For example,

helm install my-release -f values.yaml bitnami/node-exporter

**Tip: **You can use the default values.yaml

**Configuration and installation details**

It is strongly recommended to use immutable tags in a production environment. This ensures your deployment does not change automatically if the same tag is updated with a different image.

Bitnami will release a new chart updating its containers if a new version of the main container, significant changes, or critical vulnerabilities exist.

**Upgrading**

**Run this command**

helm upgrade my-release bitnami/node-exporter


**Configuration and installation details:
**
It is strongly recommended to use immutable tags in a production environment. This ensures your deployment does not change automatically if the same tag is updated with a different image.
Bitnami will release a new chart updating its containers if a new version of the main container, significant changes, or critical vulnerabilities exist.

**Setting Pod's affinity**

This chart allows you to set your custom affinity using the XXX.affinity parameter(s). Find more information about Pod's affinity in the kubernetes documentation.

As an alternative, you can use of the preset configurations for pod affinity, pod anti-affinity, and node affinity available at the bitnami/common chart. To do so, set the podAffinityPreset, XpodAntiAffinityPreset, or nodeAffinityPreset parameters.

**Troubleshooting:**

**Upgrading:**

helm upgrade my-release bitnami/node-exporter


**To 2.1.0**

This version introduces bitnami/common, a library chart as a dependency. More documentation about this new utility could be found here. Please, make sure that you have updated the chart dependencies before executing any upgrade.

**To 2.0.0**

On Nov 13,2020, Helm v2 support was formally finished, this major version is the result of the required changes applied to the Helm Chart to be able to incorporate the different features added in Helm v3 and to be consistent with the Helm project itself regarding the Helm v2 EOL.

**Upgrading to a new version**

If a new version of a helm chart is available, you are alerted in your Schematics workspace. To upgrade to a new version, complete the following steps:
1-Go to the Navigation menu > Schematics.

2- Select your workspace name.

3-Click Settings. In the Summary section, your version number is displayed. If an update is available, the Update button is displayed.

4- Click Update.

5- Select a version, and click Update.

**Uninstalling**

To uninstall a helm chart from your account, complete the following steps:
1- Go to the Navigation menu > Schematics.
2- Select your workspace name.
3- Select Actions > Destroy resources. This deletes all resources in your workspace, but it doesn't delete the workspace.
4- To delete your workspace, select Actions > Delete workspace.



