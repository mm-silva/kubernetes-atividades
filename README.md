## Atividade

Subir dois pods, nginx e mysql, mapeando a porta 80 do nginx para acesso externo ao cluster e permitir que o contêiner do nginx tenha comunicação de rede no contêiner mysql pela porta 3306. 
A atividade pode ser feita localmente (minikube), AKS (Azure), EKS (AWS) ou no GKE (GCP). 
Se quiser criar o cluster nuvem Kubernetes com Terraform é opcional. 

## Comandos importantes para o funcionamento:

git clone https://github.com/mm-silva/kubernetes-atividades.git

cd kubernetes-atividades/terraform/

terraform init

terraform plan

terraform apply -auto-approve

az aks get-credentials --resource-group ResourceGroup --name KubernetesCluster

cd ..

kubectl apply -f pods

kubectl apply -f services

kubectl get all



## Miqueias Meneses - MBA em Engenharia de software - Infrastructure and Cloud Computing
