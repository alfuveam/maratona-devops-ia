# maratona-devops-ia


O processo de criação de release da aplicação kube-news ainda é feito de forma manual. Então vamos implementar uma pipeline de CI para fazer o processo de criação da release.

Requisitos da pipeline:

A pipeline deve ser criada utilizando GitHub actions

O resultado final da pipeline deve ser uma imagem Docker no repositório do Docker Hub fabriciosveronez/kube-news-maratona e a tag deve ser definida com o número de execução do workflow no GitHub actions.

Utilize o dockerfile @02-kube-news/src/Dockerfile para construir a imagem Docker

Para a criação das actions dê sempre preferência para o uso de actions e não de comandos bash ou powershell

Crie o workflow com a pipeline de CI.

#Grafana

Obter a senha do admin
kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
