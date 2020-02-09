# openhack-gitops

### Pre-requisite 
#     K8s Cluster
#     Ingress router [for DevOps application]
#     DNS address

### Installation instruction
#     All source files for installation listed in "pre-setup" directory.
#     Install argocd, argorollout and cli using the commands listed in 0-argo_setup.txt.
#     Configure the DNS to access the argocd over the internet.
#     Using kubectl command create namespaces.
#     login to argocd using cli and also logon to argocd UI.
#     run the file 2-istio-setup.yaml  to deploy istio configuration 
#     Frist sync istio-init helm chart first. Up on successful completion, sync the istio-config helm later.
#     execute the file 3-devopstools-setup.yaml to deploy jenkins,sonarqube and harbor to devopstools namespace
#     Configure the Jenkins and update credentials for git and docker and create a pipeline using Jenkinsfile located in repo https://github.com/naveenkumarsp/gitops-argocd-demo
#     CI pipeline can build containers and push it to docker repository
#     Deploy argo example application to experience the gitops using argocd using 4-argoapps-demo.yaml
#     Deploy istio example application to experience the gitops using argocd using 5-istioapps-demo.yaml