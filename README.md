# curso-google-kubernetes-engine
 
Google Container Registry API = É igual o DockerHub, onde você armazena as imgs do docker nna nnuvem do Google

docker tag webapp gcr.io/lab-gke-438519/webapp = deixando a tag na imagem, um padrao é deixar o nome da image com o nome do laboratorio do projeto 

 gcloud projects list = lista todos os projetos na nuvem 


 kubectl get events = lista todos os evennntos


 kubectl logs pod/[nome do pod] = mostra todos os logs dos pods

 kubectl logs pod/[nome do pod] | grep teste = mostra todos os logs e marca a palavra teste

 kubectl port-forward nginx 8080:80 = esse comando vai expor o pod na porta 8080

 kubectl get pods -o wide = mostra todos os pods e os nós em que eles estão 

 