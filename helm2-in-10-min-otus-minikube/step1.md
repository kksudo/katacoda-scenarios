# Готовим окружение

1. Запускаем скрипт для подготовки переменных для доступа к kubernetes и старта minikube `minikube start`{{execute}}
    1. Проверяем, что у нас есть доступ к kubernetes кластеру `kubectl get nodes`{{execute}}
        1. В выводе должна быть хотя бы одна запись с нодой
1. Устанавливаем клиент для helm     
   `curl -LO https://storage.googleapis.com/kubernetes-helm/helm-v2.17.0-linux-amd64.tar.gz
tar -zxvf helm-v2.17.0-linux-amd64.tar.gz
mv linux-amd64/helm /usr/bin/helm`{{execute}}
1. Устанавливаем серверную часть `helm init`{{execute}}
    1. Проверяем установился ли helm `helm version`{{execute}}  
       В выводе должна быть указана версия HELM на сервере и локальная
       `Client: &version.Version{SemVer:"v2.17.0", GitCommit:"a690bad98af45b015bd3da1a41f6218b1a451dbe", GitTreeState:"clean"}
Server: &version.Version{SemVer:"v2.17.0", GitCommit:"a690bad98af45b015bd3da1a41f6218b1a451dbe", GitTreeState:"clean"}`     
       Если серверная часть возвращает ошибку, то нужно подождать пока поднимутся поды.
