# Деплоим приложение
## Ищем подходящий HELM chart

1. Добавляем публичный репозиторий, откуда будем брать наш чарт `helm repo add bitnami https://charts.bitnami.com/bitnami`{{execute}}
1. Обновляем данные из нового helm репозитория `helm repo update`{{execute}}
1. Ищем доступные чарты для установки `helm search nginx`{{execute}}    
    В выводе должен быть чарт `bitnami/nginx`   
