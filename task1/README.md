# Задание №1
Использую minikube, докер образы загружают в локальное хранилище minikube.


Для доступа к апи веб-приложение добавил абстракцию ingress.


Для поднятия окружения нужно запустить скрипт `start.sh` из корня проекта.


Чтобы сделать запрос к апи из вне, выполняем команду `minikube ip`, дальше делаем запросы по полученному ip.
*Например* `curl http://<minikube-ip>/time`.