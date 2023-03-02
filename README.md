
# Описание:
Проект api_yatube - это учебный проект API социальной сети, из курса Python-разработчик от Яндекс-Практикум.
Реализованы задачи по обеспечению взаимодействия с серверным приложением посредством API.

# Установка:
## Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:RealTheOne/api_final_yatube.git
cd api_final_yatube
```
## Cоздать и активировать виртуальное окружение:
Требуется версия Python 3.9
Активация для Windows
```
py -3.9 -m venv venv 
source venv/Script/Activate
```
## Установить зависимости из файла requirements.txt:
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
## Выполнить миграции:
```
python manage.py makemigrations
python manage.py migrate
```
## Запустить проект:
```
python manage.py runserver
```

# Примеры:
## Некоторые запросы:
### Получить список всех постов (GET):
```
http://127.0.0.1:8000/api/v1/posts/
```
### Получить список всех групп (GET):
```
http://127.0.0.1:8000/api/v1/groups/
```
### Создать новый пост (POST):
```
http://127.0.0.1:8000/api/v1/posts/

```
## Все запросы можно посмотреть в документации, по адресу:
```
http://127.0.0.1:8000/redoc/
```
