# Проект "API для Yatube"

# Описание проекта

API Yatube позволяет публиковать пользователям блоги.
Функционал проекта включает в себя создание групп для блогов,
пользователи могут оставлять комментарии к блогам,
пользователи имеют возможность подписываться друг на друга.
Для создания постов, комментариев и подписки необходима аутентификация пользователя.

## Используемые технологии и утилиты

-PYTHON
-DJANGO
-DJANGO REST
-JWT
-SQLITE

-POSTAMN

## Библиотеки и версии

```
Django==3.2.16
djangorestframework==3.12.4
djangorestframework-simplejwt==4.7.2
Pillow==9.3.0
PyJWT==2.1.0
requests==2.26.0
isort==5.12.0
```

## Запуск проекта

# Клонировать репозиторий

```
git clone git@github.com:
```

# Cоздать виртуальное окружение:

```
python -m venv venv
```

# Активировать виртуальное окружение:

```
Если у вас Windows
source venv/scripts/activate
    
Если у вас Linux/macOS
source env/bin/activate
```

# Обновить менеджер пакетов pip

```
python -m pip install --upgrade pip
```

# Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

# Выполнить миграции:

```
python manage.py migrate
```

# Дополнительная документация проекта:

```
http://127.0.0.1:8000/redoc/
```

# Запустить проект:

```
python manage.py runserver
```

# Примеры запросов:

<font color="green">Получить список всех постов:</font>

```
GET /api/v1/posts/
```

<font color="yellow">Добавление нового поста:</font>
```
POST /api/v1/posts/
```

<font color="green">Получить список всех групп:</font>
```
GET /api/v1/groups/
```

<font color="yellow">Добавление нового комментария:</font>
```
POST /api/v1/posts/{post_id}/comments/
```
<font color="orange">Удаление комментария по id:</font>
```
DELETE /api/v1/posts/{post_id}/comments/{id}/
```

<font color="green">Получение списока подписок:</font>
```
GET /api/v1/follow/
```

<font color="yellow">Подписка пользователя на пользователя переданного в запросе:</font>
```
POST /api/v1/follow/
```
