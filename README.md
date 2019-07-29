# drf-bp
Boilerplate for Django REST framework


Pre-requirement:
       
       python 3.7.4
       Django 2.2.3
       pipenv
Step1: Create project directory named "drf"

              mkdir drf
              cd drf
              
Step2: Install python packages using pipenv.
              syntax: pipenv install <package-name>
       
       pipenv shell
       pipenv install djangorestframework 
       pipenv install markdown
       pipenv install django-filter
       pipenv lock
       
Step3: Create project named "boilerplate" in the current directory.
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

Step4: Create first app named "customer"
       syntax: python manage.py startapp <app-name>
  Before creating the app make sure that you are in same directory where the file "manage.py" is present.
       
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

Step5: Create second app named "polls"
              syntax: python manage.py startapp <app-name>
       Before creating the app make sure that you are in same directory where the file "manage.py" is present.
              
              python manage.py startapp polls
       
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
       ├── Pipfile.lock
       └── polls
           ├── admin.py
           ├── apps.py
           ├── __init__.py
           ├── migrations
           │   └── __init__.py
           ├── models.py
           ├── tests.py
           └── views.py
Step6: Now sync your database for the first time
              
              python manage.py migrate
Step7:  create an initial user named "admin1" with a password of "password123"
              syntax: python manage.py createsuperuser --email <email> --username <username>
       
       python manage.py createsuperuser --email arun92saanthi@gmail.com --username admin1
Step8: 
