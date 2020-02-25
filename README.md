# aks-k8s

Requirements:
- F5 BIG-IP deployed in Azure with a public IP mapped to an IP on the BIG-IP with 80/443 open on the NSG
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
- there is two options for AS3 declarations for HTTP and one for HTTPS with and HTTP redirect. Just change the VIP IP to whatever you have on your BIG-IP

Reference: F5 Container Ingress Services - Kubernetes - https://clouddocs.f5.com/containers/v2/kubernetes/