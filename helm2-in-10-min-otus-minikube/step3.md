# Деплоим приложение
## Устанавливаем нужный HELM chart

1. Устанавливаем nignx из публичного чарта `helm install --name demo-nginx bitnami/nginx --version 7.1.6`{{execute}}   
   Нас интересует версия `7.1.6`, она имеет совместимость с версией helm2
   Команда должна завершиться без ошибок, в выводе будет справочная информация  
    ```bash
    NAME:   demo-nginx
    LAST DEPLOYED: Fri May 14 14:26:08 2021
    NAMESPACE: default
    STATUS: DEPLOYED
    ...
    ```
