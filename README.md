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
