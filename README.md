# Docker Nginx & PostgreSQL

Этот репозиторий содержит Docker-образы для **Nginx** на базе Alpine и **PostgreSQL** с автоматическим созданием пользователя и базы данных.

## Структура

```
├── nginx
│   ├── Dockerfile
│   └── nginx.conf
├── postgresql
│   └── Dockerfile
└── README.md
```

## Nginx

### Сборка и запуск

```bash
cd nginx
docker build -t custom-nginx .
docker run -d -p 80:80 --name my-nginx custom-nginx
```

## PostgreSQL

### Сборка и запуск

```bash
cd postgresql
docker build -t custom-postgres .
docker run -d -p 5432:5432 --name my-postgres custom-postgres
```