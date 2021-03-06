# newbieapis

Writing apis with Django Rest framework step by step.

### Install packages

`pip install -r requirements.txt`

### Set up a new project with a single application

```
django-admin startproject tutorial .
cd tutorial
django-admin startapp quickstart
```

The project layout should look like
```
|-- manage.py
|-- requirements.txt
`-- tutorial
    |-- __init__.py
    |-- asgi.py
    |-- quickstart
    |   |-- __init__.py
    |   |-- admin.py
    |   |-- apps.py
    |   |-- migrations
    |   |   `-- __init__.py
    |   |-- models.py
    |   |-- tests.py
    |   `-- views.py
    |-- settings.py
    |-- urls.py
    `-- wsgi.py
```

### Add new app to `INSTALLED_APPS`

Edit the MY_Project/settings.py
```
INSTALLED_APPS = [
    ...
    'rest_framework',
    'my_app.apps.My_appConfig',
]
```

### Commands

Apply updates
- `python manage.py migrate`

Create an initial user named `admin` with a password of `123456`
- `python manage.py createsuperuser --email admin@example.com --username admin`




