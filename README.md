# Python Basic
 We assume you have your Django archive and python installed on your computer.
 First, PATH verification.

On some version of windows (windows 7) you might need to make sure the Path system variable has the path the following C:\Python34\;C:\Python34\Lib\site-packages\django\bin\ in it, of course depending on your Python version.
Then, extract and install Django.


```
 c:\>cd c:\Django-x.xx
```
## Next, install Django by running the following command for which you will need administrative privileges in windows shell "cmd" −
```
 c:\Django-x.xx>python setup.py install
```

## To test your installation, open a command prompt and type the following command −

```
 c:\>python -c "import django; print(django.get_version())"
```


## If you see the current version of Django printed on screen, then everything is set.

OR

## Launch a "cmd" prompt and type python then −

```
 c:\> python
 >>> import django
 >>> django.VERSION"
```
 
## Launch a "cmd" prompt and type python then :
```
 python
```

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

#### Goto you setting.py file and the DATABASES PART REPLACE BY THIS CODE 
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

 

