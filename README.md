# api_final
## Описание проекта:
Yatube - новая социальная сеть, стремительно набирающая популярность во всём мире.  
Функционал Yatube позволяет публиковать посты, оставлять комменарии, а так же подписываться на любимых авторов.  
Yatube имеет свой собственный API, позволяющий внешним приложениям и сервисам взаимодействовать с проектом.  

### Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram2plus.git
```

```
cd kittygram2plus
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

### Примеры запросов к API:

Запрос на получение списка постов:

```
GET /api/v1/posts/
```

Создание публикации:

```
POST /api/v1/posts/
```

Получить post по id:

```
GET /api/v1/posts/{id}/
```

Получение комментариев:

```
GET /api/v1/posts/{post_id}/comments/
```

Добавление комментария:

```
POST /api/v1/posts/{post_id}/comments/
```

Список сообществ:

```
GET /api/v1/groups/
```

Список сообществ:

```
GET /api/v1/groups/
```

Список подписок пользователя:

```
GET /api/v1/follow/
```

Подписаться на пользователя:

```
POST /api/v1/follow/
```

### Использованные технологии:
Python 3.9  
Django 3.2  
DRF  
JWT + Djoser  


### Автор проекта:
Холмаков Захар
