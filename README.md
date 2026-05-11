# Дипломный практикум в Yandex.Cloud

## Kubernetes

Структура проекта:

```
.
├── helm
│   ├── diploma-app
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   │   ├── deployment.yml
│   │   │   ├── ingress.yml
│   │   │   └── service.yml
│   │   └── values.yaml
│   ├── ingress-nginx
│   │   └── values.yaml
│   └── monitoring
│       └── values.yaml
├── img
│   ├── 1.jpg
│   ├── 2.jpg
│   ├── 3.jpg
│   └── 4.jpg
├── manifests
│   └── mysql
│       ├── deployment.yml
│       └── service.yml
└── README.md
```

Данный репозиторий содержит манифесты Kubernetes для развертывания мониторинга кластера и приложения используя Dockerfile при помощи Nginx

Для корректной работы необходимо иметь и обновлять секрет **KUBE_CONFIG** при помощи команды `ssh user@k8s-master "cat ~/.kube/config" | base64 -w 0; echo`

Результат выполнения пайплайна:

![Ответ на задание 1](https://github.com/Francotirado/diploma-k8s/blob/main/img/1.jpg)

Развернутый мониторинг и пользовательское приложение:

![Ответ на задание 1](https://github.com/Francotirado/diploma-k8s/blob/main/img/2.jpg)

![Ответ на задание 1](https://github.com/Francotirado/diploma-k8s/blob/main/img/3.jpg)

![Ответ на задание 1](https://github.com/Francotirado/diploma-k8s/blob/main/img/4.jpg)
