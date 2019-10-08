# django_pages_app
• create a new directory for our code
• install Django in a new virtual environment
• create a new Django project
• create a new pages app
• update settings.py

command line
$ cd ~/Desktop
$ mkdir pages_app
$ cd pages_app
$ pipenv install django
$ pipenv shell
(pages_app) $ django-admin startproject pagesapp .
(pages_app) $ python manage.py startapp pages

# pages_project/settings.py
INSTALLED_APPS = [
'pages.apps.PagesConfig', # new
'django.contrib.admin',
'django.contrib.auth',
'django.contrib.contenttypes',
'django.contrib.sessions',
'django.contrib.messages',
'django.contrib.staticfiles',
]

(pages_app) $ python manage.py runserver
