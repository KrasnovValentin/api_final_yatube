# api_final

## Спринт 9. api_yatube. Финальная реализация API для проекта **Yatube**.

### Описание.
Проект API для yatube-соцсети в которой пользователи могут публиковать свои
статьи, оставлять комментарии под статьями, подписываться на понравившихся 
авторов.

### Как запустить проект:  
Клонировать репозиторий и перейти в него в командной строке:

#### Cоздать и активировать виртуальное окружение:  
 `python3 -m venv env`  
 `source env/bin/activate`
 
 Установить зависимости из файла *requirements.txt*:  
`python3 -m pip install --upgrade pip`  
`pip install -r requirements.txt`

Выполнить миграции:  
`python3 manage.py migrate`

Запустить проект:  
`python3 manage.py runserver`

### Примеры запросов к API.
Запрос **GET**  
http://127.0.0.1:8000/api/v1/posts/ - просмотреть все статьи.  
Запрос **POST**  
http://127.0.0.1:8000/api/v1/posts/ - опубликовать статью  
Запрос **GET**  
http://127.0.0.1:8000/api/v1/posts/{id}/ - просмотреть подробности одной статьи  
Запрос **POST**  
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/ - добавить  
комментарий к выбранному посту
Запрос **GET**  
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/ - просмотреть все 
комментарии к выбранному посту
Запрос **GET**  
http://127.0.0.1:8000/api/v1/groups/ - просмотреть список сообществ
Запрос **GET**  
http://127.0.0.1:8000/api/v1/groups/{id}/ - просмотреть информацию о конкретном
 сообществе
Запрос **GET**  
Запрос **POST**  
http://127.0.0.1:8000/api/v1/follow/ - подписаться на конкретного автора или 
получить список своих подписок

---
#### Стек технологий: Python, Django REST framework
