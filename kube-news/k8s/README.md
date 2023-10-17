********************** DESAFIO ************************
Rodar os comandos abaixo para realizar o deploy do pod/imagem do banco e app
Modificada a porta do popula-dados.http para que a chama rest execute.
*******************************************************

k3d cluster create meucluster -p "8080:30000@loadbalancer"

cd imersao-devops-cloud-02/kube-news/

kubectl apply -f k8s/deployment.yaml
