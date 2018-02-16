# Service Fabric Cluster with Reverse Proxy

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Overview

This template allows to deploy a secure Service Fabric Cluster which is improved to host the Web applications.

This template utilizes Reverse Proxy for HTTP traffic routing to the Web applications hosted on the cluster.

This template provides secure access to the cluster via Azure Active Directory.

## Prerequisites


### Azure Key Vault

Azure Key Vault is used as a safe storage location for certificates and as a way to get certificates installed on Service Fabric clusters in Azure.

**ClusterCertificate** - This certificate is required to secure the communication between the nodes on a cluster.

**ReverseProxyCertificate** - This SSL certificate is required to secure a reverse proxy.

[Read More](https://docs.microsoft.com/en-us/azure/security/azure-service-fabric-security-overview) about the Azure Service Fabric security.

### Azure Active Directory

Azure Acitev Directory provides Identification and Authontication for users which want to manage the cluster.

**Fabric Web Manager** - a web-based application that provides management of the Service Fabric cluster.

**Fabric Native Manager** - a native client experience that provides management of the Service Fabric cluster.
