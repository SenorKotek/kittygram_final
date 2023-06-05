#  Социальная сеть для котиков Kittygram

## URL изначального проекта

Изначальный проект развернут на сайте https://imacatmlem.ddns.net/

## Запуск проекта в Dev-режиме

Клонируйте репозиторий, создайте базу и .env под нее

В папке с проектом запустите команду

docker compose up

Запустятся контейнеры:
- kittygram_backend
- kittygram_frontend
- kittygram_gateway
- db

Cоберите и скопируйте статику
```
docker compose exec backend python manage.py collectstatic
```
```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```

Проект будет доступен по адресу 
```
loсalhost:9000
```

### Автор

SenorKotek