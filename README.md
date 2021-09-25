[![Django-app Actions Status](https://github.com/vlad397/yamdb_final/workflows/Django-app/badge.svg)](https://github.com/vlad397/yamdb_final/actions)
# api_yamdb
### Описание
API с возможностью просматривать существующие в базе категории, жанры и тайтлы на различного рода медиа объекты, оставлять к ним комментарии и давать оценки
### Запуск проекта
Проект доступен в Docker репозитарии по адресу _https://hub.docker.com/r/vlad397/infra_sp2_web_
После загрузки контейнера на локальную машину выполните следующие команды:
```docker-compose up``` *для развертывания проекта*
```docker-compose exec web python manage.py makemigrations``` --noinput *для создания миграций*
```docker-compose exec web python manage.py migrate --noinput``` *для применения миграций*
```docker-compose exec web python manage.py createsuperuser``` *для создания суперпользователя*
```docker-compose exec web python manage.py collectstatic --no-input``` *для подгрузки статики*
Проект доступен по адресу _http://127.0.0.1/api/v1/_
Админка доступна по адресу _http://127.0.0.1/admin/_
Для создания тестовых данных откройте админку, залогиньтесь через суперпользователя и добавляйте необходимые данные.
В качестве примера можете открыть проект автора, который доступен по адресу _http://84.252.138.253_