# mypoc-helmchart-k8s
## Setting up istio helm chart 
### Configure the helm repository

$ helm repo add istio https://istio-release.storage.googleapis.com/charts

$helm search repo istio

$ helm repo update

### Download helm chart for Istio locally

helm pull istio/istiod --untar      -- Helm chart for istio control plane

helm pull istio/base --untar        --Helm chart for deploying istio cluster resource

helm pull istio/cni --untar         --Helm chart for istio-cni components

helm pull istio/gateway --untar     --Helm chart for deploying istio gateways

##Configuring microservice example
Here I am configuring helm chart for microservices which are available at https://github.com/GoogleCloudPlatform/microservices-demo.git

Thia example is mainly demonstrating helm chart for complex microservice but we are additionally doing argo cd setup


