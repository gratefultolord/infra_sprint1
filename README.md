# infra_sprint1
Данный проект представляет собой площадку для публикации данных о котах, включая их имя, год рождения, цвет, владельца и достижения.

**Инструменты и стек:** #Python #Django #Docker-compose #API #Nginx #Pillow #Djoser #Gunicorn #Python-dotenv #JSON #YAML #Postman #PyCharm

## Запуск
Для запуска приложения необходим сервер, рассмотрим на примере сервера под управлением ОС Linux.

1. Подготовим виртуальное окружение в директории проекта создадим файл .env:
```bash
nano .env
```

2. Переписываем файл /etc/nginx/sites-enabled/default на основе infra/default
3. Создаем файл gunicorn_kittygram.service из аналогичного файла в папке infra
4. Перезапускаем gunicorn и nginx
5. Проект работает

## Примеры запросов

Добавить питомца: POST `/cats/add`

Редактировать питомца: PUTCH `/cats/edit`

Просмотр питомца: GET `/cats/{cat_id}`
