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


 