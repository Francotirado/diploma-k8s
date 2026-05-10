# Дипломный практикум в Yandex.Cloud

## Kubernetes

Структура проекта:

```
.
├── .github
│   └── workflows
│       └── deploy.yml
├── helm
│   ├── ingress-nginx
│   │   └── values.yaml
│   └── monitoring
│       └── values.yaml
├── manifests
│   └── app
│       ├── deployment.yml
│       ├── ingress.yml
│       └── service.yml
├── README.md
└── scripts
```

Данный репозиторий содержит манифесты Kubernetes для развертывания мониторинга кластера и приложения используя Dockerfile при помощи Nginx
