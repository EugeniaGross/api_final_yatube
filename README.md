### Описание проекта:
API социальной сети - блога, с возможностью публикации, редактирования, удаления постов и комментариев, получение информации о сообществах и подписках.

### Запуск проекта:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```
### Примеры:
### Получение списка сообществ api/v1/groups/
[
  {
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
  }
]
### Получение публикации api/v1/posts/{id}/
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
