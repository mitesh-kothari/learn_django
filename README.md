# Django notes
### How to install Django
* To install Django first we need python.
* create virtual environment.
  * ``python -m venv <virtual environment folder name>``


* activate virtual env.
  * ``cd myproject\Scripts\activate.bat``


* Now every package we install will locate in venv(virtual environment), install Django in venv.
  * ``py -m pip install Django``


* check Django version.
  * ``django-admin --version``


* Now create a project at folder root where your venv folder located.
  * ``django-admin startproject <project folder name>``


* serve the project.
  * manage.py provide command line utility so every command of django we execute from folder where manage.py located (project root).
  * ``py manage.py runserver``


* create requirement.txt
  * We can use ``pip list`` or ``pip freeze`` to see installed packages.
  * ``pip freeze > requirements.txt``


* install dependency from requirement.txt
  * ``pip install -r requirements.txt``
  * List outdated packages ``pip list --outdated``
  * Update a package ``pip install -U fastapi``
  * Check for missing dependencies ``python -m pip check``

* Migrate to database ``py manage.py migrate``


* create migration from models ``py manage.py makemigrations <model name>``


* Show sql from migration ``py manage.py sqlmigrate polls 0001``


* python shell ``py manage.py shell``


* Create Django ``py manage.py createsuperuser``