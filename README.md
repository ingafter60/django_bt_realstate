# BUILDING A REAL-ESTATE WEB APPLICATION USING DJANGO V.2.2

## 01. Getting Started

### 01.1.1 - Initial setup

        new file:   .gitignore
        new file:   REACME.md

### 01.2.2 - Create django project

		> Create virtual environment 'venv3822'
		> Activate venv3822
		> Install django v.2.2
		> Create django project inside the root folder 'config' 
		> Run the server to test it out
		>> python manage.py runserver
		> DONE:)
        modified:   .gitignore
        modified:   README.md
        new file:   config/__init__.py
        new file:   config/__pycache__/__init__.cpython-38.pyc
        new file:   config/__pycache__/settings.cpython-38.pyc
        new file:   config/__pycache__/urls.cpython-38.pyc
        new file:   config/__pycache__/wsgi.cpython-38.pyc
        new file:   config/settings.py
        new file:   config/urls.py
        new file:   config/wsgi.py
        new file:   db.sqlite3
        new file:   manage.py

### 01.3.3 - Setting up MySQL Database and create superuser

		> Install mysqlclient
		> Create database 'django_bt_realstate'
		> Setup the database credentials in settings
		DATABASES = {
		    'default': {
		        'ENGINE': 'django.db.backends.mysql',
		        'NAME': "django_bt_realstate",
		        'USER': 'root',
		        'PASSWORD': '',
		        'PORT': 3306
		    }
		}
		> Run the server to test it out
		> Run migrations
		> Create superuser
		> The results
		mysql> CREATE DATABASE django_bt_realstate;
		Query OK, 1 row affected (0.49 sec)
		mysql> USE django_bt_realstate;
		Database changed
		mysql> show tables;
		+-------------------------------+
		| Tables_in_django_bt_realstate |
		+-------------------------------+
		| auth_group                    |
		| auth_group_permissions        |
		| auth_permission               |
		| auth_user                     |
		| auth_user_groups              |
		| auth_user_user_permissions    |
		| django_admin_log              |
		| django_content_type           |
		| django_migrations             |
		| django_session                |
		+-------------------------------+
        modified:   README.md
        modified:   config/__pycache__/settings.cpython-38.pyc
        modified:   config/settings.py