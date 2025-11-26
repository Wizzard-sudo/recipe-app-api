# recipe-app-api
Recipe API Project

generate a project
docker-compose run --rm app sh -c "django-admin startproject app ."

generate new module:
docker-compose run --rm app sh -c "python manage.py startapp core"

generate migrations:
docker-compose run --rm app sh -c "python manage.py makemigrations"




run linting:
docker-compose run --rm app sh -c "flake8"

run unit tests:
docker-compose run --rm app sh -c "python manage.py test"

run command:
docker-compose run --rm app sh -c "python manage.py wait_for_db"

run migrations:
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

create superuser:
docker-compose run --rm app sh -c "python manage.py createsuperuser"