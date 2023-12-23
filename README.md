# Python Basic 

## Show Python Command :
```
 django-admin
```

## Create Project

```
django-admin project_name
```
here project_name is your project name. You can use any valid name as a project name.

## Run python server
```
py manage.py runserver
```
## Create python app
```
py manage.py startapp appname
```
Here appname is any valid name for python app

## Create migration 
```
py manage.py makemigrations
```
## Run migrations
```
py manage.py migrate

### Run Migration by Migration Name

py manage.py sqlmigrate app_name migration_name
```

## install mysql database page with python prject
```
pip install mysqlclient
```

## Add mysql database with python project

Goto you setting.py file and the DATABASES PART REPLACE BY THIS CODE 
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'funclubdb',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

 

