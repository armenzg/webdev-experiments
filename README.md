# Webdev experiments

This repository is to experiment with various web development concepts around ReactJs and Django.
The `master` branch will not have much besides listing the various concepts implemented
on a different branch.

## Requirements

This project will only focus on some set of recommended tools and versions. All others will not be discussed to simplify the documentation.

* Python 3
* Django 2
* pipenv

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
