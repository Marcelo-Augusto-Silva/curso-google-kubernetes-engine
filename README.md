# curso-google-kubernetes-engine
 
Google Container Registry API = É igual o DockerHub, onde você armazena as imgs do docker nna nnuvem do Google

docker tag webapp gcr.io/lab-gke-438519/webapp = deixando a tag na imagem, um padrao é deixar o nome da image com o nome do laboratorio do projeto 

 gcloud projects list = lista todos os projetos na nuvem 


 kubectl get events = lista todos os evennntos


 kubectl logs pod/[nome do pod] = mostra todos os logs dos pods

 kubectl logs pod/[nome do pod] | grep teste = mostra todos os logs e marca a palavra teste

 kubectl port-forward nginx 8080:80 = esse comando vai expor o pod na porta 8080

 kubectl get pods -o wide = mostra todos os pods e os nós em que eles estão 






Parte 2 do curso

Tipos de estrategias de deploy 

Rolling update = Vai atualizando um container por vez 

Blue / Green = Mantem duas infraestrutura, uma azul e uma verde, voce muda da azul para verde, voce mantem as duas infraestruturas porque assim você pode reverter

CANARY = Voce faz deploy em alguns pods e depois vai validando, se estiver validado, voce aplica para outros pods


gcloud container clusters create-auto guestbook --region us-east1  = Esse comando cria um cluster com o nome guestbook na regiao us-east1



kubectl get svc -n kube-system = lista todos os serviços do namespace kube-system 

kubectl apply -f https://k8s.io/examples/admin/dns/dnsutils.yaml = URL do DNS sutil


kubectl exec -it [nome do container] -- /bin/bash = comando para rodar o bash dentro de um container



dig redis-leader.default.svc.cluster.local = esse comando serve para fazer uma consulta no DNS local do cluster esse comando rodei dentro do container que eu subi na linha 35

dig [nome do servico].[namespace].[svc ou pod].[cluster].[local]

    