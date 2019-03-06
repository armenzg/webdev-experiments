# Webdev experiments

This repository is to experiment with various web development concepts around ReactJs and Django.
The `master` branch will not have much besides listing the various concepts implemented
on a different branch.

## Requirements

This project will only focus on some set of recommended tools and versions. All others will not be discussed to simplify the documentation.

* Python 3
* Django 2
* pipenv

## Summary

What you will find in the following sections:

* Set up Django
* Server Django app via Gunicorn

## Django set up work

On this branch we have a Django Hello World app.

Steps followed:

```bash
# Create virtual environment
pipenv --three
# Install the Django library
pipenv install Django
# Create your Django project
pipenv run django-admin startproject mysite
```

Run development server:

```bash
pipenv run mysite/manage.py runserver
```

Load the page by visting [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Gunicorn

Django does not come with a production ready Http server.
This adds Gunicorn to serve the app.
Gunicorn (‘Green Unicorn’) is a pure-Python WSGI server for UNIX. It has no dependencies and is easy to install and use.

Setup steps:

```bash
pipenv install gunicorn
```

Run the server:

```bash
cd mysite
pipenv run gunicorn mysite.wsgi
```

Load the page by visting [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
