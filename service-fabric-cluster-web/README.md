# Service Fabric Cluster for Web Apps

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Overview

This template allows to deploy a secure Service Fabric Cluster which is improved to host the Web applications.

This template utilizes Application Gateway to provide HTTP traffic routing to the Web applications hosted on the cluster.

This template utilizes Service Fabric Reverse Proxy service to route HTTP traffic within the cluster.

This template assumes that you already have certificates uploaded to your keyvault.

## Prerequisites

### Azure Key Vault

**ClusterCertificate** - This certificate is required to secure the communication between the nodes on a cluster.

**ServerCertificate** - This certificate is required to connect to a cluster.

**ReverseProxyCertificate** - This certificate is required to secure a reverse proxy.

[Read More](https://docs.microsoft.com/en-us/azure/security/azure-service-fabric-security-overview) about the Azure Service Fabric security.

### Azure Active Directory

Azure Acitev Directory provides Identification and Authontication for users which want to manage the cluster.

**Fabric Web Manager** - a web-based application that provides management of the Service Fabric cluster.

**Fabric Native Manager** - a native client experience that provides management of the Service Fabric cluster.
