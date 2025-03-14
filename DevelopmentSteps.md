# Sarvagya - Development Steps

## Pre-Requisites

1. Python 3.12
2. SQL Server
3. Open AI API key
4. VS Code
5. Git

## Project Setup

1. Create and activate python virtual environment
2. Install django, django drf, python-dotenv, mssql-django, and openai
```sh
pip install django djangorestframework python-dotenv mssql-django openai
```
3. Create a django project `Sarvagya`
```sh
django-admin startproject Sarvagya
```
4. Create a `.env` file at project directory.
5. Load the dotenv in project `settings.py`
6. Move the sensitive contents to `.env` such as `DEBUG`, `SECRET_KEY`
7. Add `rest_framework` to `INSTALLED_APPS` in `settings.py`
8. Add sql server database settings in `DATABASES` in `settings.py`
9. Migrate db tables `python manage.py migrate`
10. Create superuser `python manage.py createsuperuser`
11. Run server and login using superuser credentails `127.0.0.1:8000/admin`