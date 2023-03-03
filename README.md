# Учебный проект API для приложения Yatube
## Описание:
Проект api_yatube - это учебный проект API социальной сети, из курса Python-разработчик от Яндекс-Практикум.
Реализованы задачи по обеспечению взаимодействия с серверным приложением Yatube посредством API. Есть возможность публиковать, читать и комментировать посты, подписываться на авторов и отписываться от них. Обеспечено разделение полномочий пользователей, в зависимости от того авторизованы они или нет.
### Использованы технологии:
1. Python 3.9
2. Django 3.2
3. DRF 3.12
4. JWT + Djoser
## Установка:
### Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:RealTheOne/api_final_yatube.git
cd api_final_yatube
```
### Cоздать и активировать виртуальное окружение:
Требуется версия Python 3.9
Активация для Windows
```
py -3.9 -m venv venv 
source venv/Script/Activate
```
### Установить зависимости из файла requirements.txt:
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
### Выполнить миграции:
```
python manage.py makemigrations
python manage.py migrate
```
### Запустить проект:
```
python manage.py runserver
```

## Примеры:
### Некоторые запросы:
Получить список всех постов (GET):
```
http://127.0.0.1:8000/api/v1/posts/
```
Ответ:
```
{

    "count": 123,
    "next": "http://api.example.org/accounts/?offset=400&limit=100",
    "previous": "http://api.example.org/accounts/?offset=200&limit=100",
    "results": 

[

        {
            "id": 0,
            "author": "string",
            "text": "string",
            "pub_date": "2021-10-14T20:41:29.648Z",
            "image": "string",
            "group": 0
        }
    ]

}
```
Получить список всех групп (GET):
```
http://127.0.0.1:8000/api/v1/groups/
```
Ответ:
```
[

    {
        "id": 0,
        "title": "string",
        "slug": "string",
        "description": "string"
    }

]
```
Создать новый пост (POST):
```
http://127.0.0.1:8000/api/v1/posts/

```
Ответ:
```
{

    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0

}
```
### Все запросы можно посмотреть в документации, по адресу:
```
http://127.0.0.1:8000/redoc/
```
## Автор:
- Идрисов Артур