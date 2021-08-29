# Django, PostgreSQL and Docker example

Virtualenv and install django

```console
$ py -m venv venv
$ .\venv\Scripts\activate

$ pip install django
```

Create project

```console
$ django-admin startproject <project_name> .
```

Create app

```console
$ django-admin startapp <app_name>
```

Run docker

```console
$ docker-compose up -d
```

Run migrate

```console
$ docker-compose exec web python manage.py migrate
```

Create superadmin

```console
$ docker-compose exec web python manage.py createsuperuser
```