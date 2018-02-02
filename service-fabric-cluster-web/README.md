# Deployment of the secure Service Fabric Cluster specialized for Web Applications

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fstas-sultanov%2FAzure-Templates%2Fmaster%2Fservice-fabric-cluster-web%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template allows you to deploy a secure Service Fabric Cluster which is improved to host the Web applications.
This template utilizes Application Gateway to provide HTTP traffic routing to the Web applications hosted on Cluster.
This template utilizes Service Fabric Reverse Proxy service to route HTTP traffic.
This template assumes that you already have certificates uploaded to your keyvault.

