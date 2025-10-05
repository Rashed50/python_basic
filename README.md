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

You can install django inside your virtual environment. Moreover Globaly, You can install django using command line. Open you power shell terminal in windows computer. Then Use this command for django installation

```
python -m pip install Django
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

## Create Virtual Environment
For creating python project first you have to create virtual environment first. so to create virtual environment first open terminal in a folder then type below command in windows computer.
Here "dj_virtual_env" is avirtual environment name

```
py -m venv dj_virtual_env
```


## Create Project

```
django-admin startproject project_name
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
py manage.py makemigrations app_name or module_name
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

## Create Required Library text file called requirements.txt  
Make sure your project's virtual environment (venv, env, etc.) is activated. This ensures that pip freeze only lists the packages specific to your project,
not every Python package installed on your computer.
Once your virtual environment is active and you are in your project's root directory (where your manage.py file is located), run the following command.
The > is a shell redirection operator that tells your system to write the output of pip freeze into the specified file.

```
pip freeze > requirements.txt
```
The generated requirements.txt file will contain a list of packages and their pinned versions, like this:

## Install bootstrap in python project

First you have to activate virtual environment if have not activate. then at inside virtual enironment folder type the below command 

```
pip install django-bootstrap-v5
```

Next step is to include the bootstrap module in the INSTALLED_APPS list in the file of  settings.py:

```
bootstrap5
```
# Django Templates

## 1. Create Vertual Invironments

#### Windows 
```bash
py -m venv env
```
#### Linux
```bash
python3 -m venv env
```


## 2. Activate Virtual Invironments

#### Windows 
```bash
env\Scripts\activate
```

#### Linux
```bash
source env/bin/activate
```



## 3. Deactivate Virtual Invironments

```bash
deactivate
```


## 4. Upgrade PIP

```bash
python.exe -m pip install --upgrade pip
```



## 5. Install Requirement Txt Files
```bash
pip install -r requirements.txt
```


## 6. Create and Copy .env file
```bash
copy .env.example .env
```


## 7. Makemigration
```bash
python manage.py makemigrations
```



## 8. Migrate
```bash
python manage.py migrate
```



## 9. Create Superuser
```bash
python manage.py createsuperuser
```
#### Email:
```bash
admin@test.com
```
#### Phone Number:
```bash
01500000001
```
#### Password:
```bash
admin
```


## 10. Now can run the Django server
```bash
python manage.py runserver
```
 

