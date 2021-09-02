# DJANGO DEMO

Before you can start to build the individual functionality of a new Django web application, you always need to complete a couple of setup steps on your machine.

1. Install python3 
2. Set up a virtual environment
3. Install Django
4. Set up a Django project
5. Start a Django app


You can check above first two requirements are install on your machine by running below command in terminal.

```
python3 --version
virtualenv --version
```

## Let's start with Django 

Go to your terminal create a directory & locate to that directory.
```
mkdir <dir_name> && cd <dir_name>
```

First we will need to create a virtual environment & activate it.
```
virtualenv venv
source venv/bin/activate
```

## Install Django

Install Django with below command:
```
python3 pip install django
```

you can check django version:
```
python3 -m pip django --version
```

## Set up a Django project

With your virtual environment set up and activated and Django installed, you can now create a project by executing startproject command:

```
django-admin startproject <project-name>
```

we used 'scrap' as project name:
```
django-admin startproject scrap
```

Running this command creates a default folder structure, which includes some Python files and your management app that has the same name as your project:

```
scrap/
│
├── scrap/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
└── manage.py
```

In the code block above, you can see the folder structure that the startproject command created for you:

finmarka/ :- is your top-level project folder.
finmarka/finmarka/ :- is your lower-level folder that represents your management app.
manage.py :- is a Python file that serves as the command center of your project. It does the same as the django-admin command-line utility.

Run below command to start django server:
```
python3 manage.py runserver
```
 
When you’re ready, you can move on to create a Django app as a lower-level unit of your new web application.

## Start a Django App
Now, you’ll create a Django App by executing the 'startapp' command through the manage.py file:
```
python manage.py startapp <appname>
```

The startapp command generates a default folder structure for a Django app. This uses 'scraper' as the name for the app:
```
python manage.py startapp scraper
```

Once the startapp command has finished execution, you’ll see that Django has added another folder to your folder structure:
```
scrap/
│
├── scraper/
│   │
│   ├── migrations/
│   │   └── __init__.py
│   │
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── scrap/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
└── manage.py
```

At this point, you’ve finished setting up for your Django web application, and you can start implementing your ideas.


