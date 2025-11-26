# recipe-app-api
Recipe API Project

generate a project
docker-compose run --rm app sh -c "django-admin startproject app ."

run linting:
docker-compose run --rm app sh -c "flake8"

run unit tests:
docker-compose run --rm app sh -c "python manage.py test"