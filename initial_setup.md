Creating Django project:
    1. create virtual env via below commands
        python -m venv <env_name>
    2. activate the venv created
        source <env_name>/bin/activate
    3. create Django project:
        django-admin startproject <project name>
    4. Create 
        README.md: To describe how to set up project or explain regarding the project
        .gitignore: To avoid some files going to remote repo
        requirement.txt: to get list of all packages used and their respective version
                         pip freeze > requirement.txt
        create template, static directory and set the path in settings.py
    5. create a app in django project
        cd <project name>
        python manage.py startapp <app_name>
        * Add this app name in settings installed app list
    6. After creating the base project then initiate git:
        git init

Some tips for take the best from django:
For Database querying:
    1. Use annote as much as possible with the help of "F" string.
    2. Use select_related, prefetch_relate to get related table fields.
    3. If there are millions of record, instead querying all once at the time do pagination.
    4. Try to cache the querying in views.py