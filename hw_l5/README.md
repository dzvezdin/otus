После установки нужно будет добавить запись в /etc/hosts с ip (minikube ip) и url arch.homework
Возможно потребуется в файле ingress.yaml убрать строку ingressClassName: nginx, но у меня без нее не работает.
Проверить работу сервиса можно:
curl http://arch.homework
curl http://arch.homework/health
curl http://arch.homework/otusapp/zvezdin/
