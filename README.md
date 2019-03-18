<!-- TITLE:  Django: Quick Start -->
<!-- SUBTITLE: Step by step installation, commands, tutorials, and resources for new Django developers. -->

# Django: Quick Start

## Installation: Step by Step

Run the following commands in your Terminal:

1. Install `python3`: `brew install python3`
1. Install `virtualenv`: `pip3 install virtualenv`
1. Create a directory for your new project: `mkdir new-project && cd new-project`
1. Create a new `virtualenv` for the new project: `virtualenv env`
1. Activate the new `virtualenv`: `source env/bin/activate`
1. Install Django in the fresh `env`: `pip install django`
1. Generate scaffolding for your new Django project: `django-admin startproject proj`
1. Navigate to the new Django project directory: `cd proj`
1. Create a new Django app: `python manage.py startapp tasks`
1. Run the Django development server: `python manage.py runserver
1. Create môi trường: `mkvirtualenv test-1 --python=/usr/bin/python3`
1. Tắt môi trường ảo: `$ deactivate`
1. Goi moi truong ao: `$ workon test-1`
1. Trong môi trường, cài đặt gói Django bằng pip: `$ pip install django`
1. Xuất các package sử dụng ra file requirements.txt
  * `$ pip3 freeze > requirements.txt`
1. Và sử dụng để cài các gói đã xuất từ requirements.txt
  * `$ pip3 install -r requirements.txt`
1. cập nhật database từ mysql về models
  * `$ python manage.py inspectdb > blog/models.py`
  
* `exec(open("./web/test_bcrypt.py").read())`
* `git reset --soft HEAD^`
* `CREATE DATABASE vna CHARACTER SET utf8 COLLATE utf8_general_ci;
* `CREATE USER 'vna'@'localhost' IDENTIFIED BY 'vna123';`
* `SET GLOBAL validate_password_length = 6;`
* `SET GLOBAL validate_password_number_count = 0;`
* `SET GLOBAL validate_password_policy=LOW;`
* `compilemessages and makemessages -l 'fr'`
## Git
* `git branch`
* `git checkout -b dev-cuong` : Tao Nhanh branch
* `git push --set-upstream origin dev-cuong` : push server
* `git chackout`
* `git merge`
## Helpful Management Commands

* `python manage.py makemigrations`: Generates migrations for newly created Django apps.
* `python manage.py migrate`: Applies migrates generated by `makemigrations`

## Tutorials
The best tutorial for Django is located within the documentation. Follow all six steps and you'll know everything you need to know to hit the ground running!

* [Writing Your First Django App: Part 1 - Getting Started](https://docs.djangoproject.com/en/2.0/intro/tutorial01/)
* [Writing Your First Django App: Part 2 - Database Setup](https://docs.djangoproject.com/en/2.0/intro/tutorial02/)
* [Writing Your First Django App: Part 3 - Views/URLs](https://docs.djangoproject.com/en/2.0/intro/tutorial03/)
* [Writing Your First Django App: Part 4 - Forms](https://docs.djangoproject.com/en/2.0/intro/tutorial04/)
* [Writing Your First Django App: Part 5 - Testing](https://docs.djangoproject.com/en/2.0/intro/tutorial05/)
* [Writing Your First Django App: Part 6 - Templates](https://docs.djangoproject.com/en/2.0/intro/tutorial06/)

## Documentation
**Full documentation located here**: https://docs.djangoproject.com/en/2.0/

* [Models: Field Reference](https://docs.djangoproject.com/en/2.0/ref/models/fields/)
* [Views: Writing Views](https://docs.djangoproject.com/en/2.0/topics/http/views/)
* [Views: URL Dispatcher](https://docs.djangoproject.com/en/2.0/topics/http/urls/)
* [Views: Shortcuts](https://docs.djangoproject.com/en/2.0/topics/http/shortcuts/)
* [Templates: Overview](https://docs.djangoproject.com/en/2.0/topics/templates/)
* [Templates: Built-in Template Tags and Filters](https://docs.djangoproject.com/en/2.0/ref/templates/builtins/)
