`api_final_yatube` представляет собой `API` для проекта Yatube.
Это `API` предназначенное для добавления, удаления, комментирования, а так же редактирования добавленных записей.


## Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:sntchweb/api_final_yatube.git
```
Cоздать и активировать виртуальное окружение:
```
py -m venv env
```
```
source env/bin/activate
```
Установить зависимости из файла requirements.txt:
```
py -m pip install --upgrade pip
```
```
pip install -r requirements.txt
```
Выполнить миграции:
```
py manage.py migrate
```
Запустить проект:
```
py manage.py runserver
```

## Примеры запросов и ответов:
```
Запрос: http://127.0.0.1:8000/api/v1/posts/1
Ответ:
{
	"id": 1,
	"author": "artem",
	"text": "test 1st text",
	"pub_date": "2023-04-03T05:58:41.224351Z",
	"image": null,
	"group": null
}

```
```
Запрос: http://127.0.0.1:8000/api/v1/posts/1/comments/
Ответ:
[
	{
		"id": 1,
		"author": "artem",
		"text": "test comment text",
		"created": "2023-04-03T06:57:15.561793Z",
		"post": 1
	}
]
```
