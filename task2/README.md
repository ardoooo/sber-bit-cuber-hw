# Задание №2
Использую minikube, докер образы загружают в локальное хранилище minikube.


Для поднятия окружения нужно запустить скрипт `start.sh` из корня проекта.


Чтобы сделать запрос к апи из вне, выполняем скрипт `get_address.sh`, дальше делаем запросы по полученным ip и порту.
*Например* `curl http://<minikube-ip>:<node-port>/time`.


Интересно было поизучать возможности lstio, можно подключить kiali для визуализации сервисов, трафика и просмотра логов.


Командой `minikube kubectl -- apply -f https://raw.githubusercontent.com/istio/istio/release-1.10/samples/addons/kiali.yaml` устанавливаем и запускам.


Чтобы запустить графический интерфейс в браузере выполняем команду `istioctl dashboard kiali`.