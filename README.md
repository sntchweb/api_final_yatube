# api_final_yatube
Что такое api_final_yatube?
Это `API` предназначенное для добавления, изменения, удаления, а так же редактирования записей.


## Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:sntchweb/api_final_yatube.git
```
Cоздать и активировать виртуальное окружение:
```
python3 -m venv env
```
```
source env/bin/activate
```
Установить зависимости из файла requirements.txt:
```
python3 -m pip install --upgrade pip
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
