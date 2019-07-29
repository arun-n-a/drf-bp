# drf-bp

python 3.7.4
Django 2.2.3
pip install pipenv

Boilerplate for Django REST framework

Step1: Install python packages using pipenv.
       syntax: pipenv install <package-name>
       pipenv install djangorestframework 
       pipenv install markdown
       pipenv install django-filter
       pipenv lock
Step2: Create project named "boilerplate" in the current directory.
       syntax: django-admin startproject <new-project-name> .
       django-admin startproject boilerplate .
  
Now the directory looks like:  .
  ├── boilerplate
  │   ├── __init__.py
  │   ├── settings.py
  │   ├── urls.py
  │   └── wsgi.py
  ├── manage.py
  ├── Pipfile
  └── Pipfile.lock

Step3: Create first app named "customer"
       syntax: python manage.py startapp <app-name>
  Before creating the apps make sure that you are in same directory where the file "manage.py" is present.
  
  python manage.py startapp customer
  
  Now the directory looks like:
    ├── boilerplate
    │   ├── __init__.py
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    ├── customer
    │   ├── admin.py
    │   ├── apps.py
    │   ├── __init__.py
    │   ├── migrations
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── tests.py
    │   └── views.py
    ├── manage.py
    ├── Pipfile
    └── Pipfile.lock
