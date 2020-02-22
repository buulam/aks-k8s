# aks-k8s

Requirements:
- F5 BIG-IP deployed in Azure
- Check that AS3 / schema version is up to date

First, install Azure CLI

From there, this should be all the commands you should need to:
- build AKS cluster
- deploy F5 Controller
- create service account and RBAC
- create secret with BIG-IP credentials
- deployment of f5-hello-world demo container
- create kubernetes Services definition
- deploy configmap with AS3 declaration
-- there is two options for AS3 declarations for HTTP and one for HTTPS with and HTTP redirect