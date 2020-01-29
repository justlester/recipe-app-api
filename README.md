# recipe-app-api

First Django REST API

Using: 
<ul>
<li>Conda</li>
<li>Python</li>
<li>MySQL</li>
</ul>

<h1>Setup Project:</h1>

Create environment for the project

```
conda create --name <environment-name> python=3.7
```

Activate environment

```
conda activate <environment-name>
```

Navigate to project directory

```
cd recipe-app-api
```

Install project requirements 

```
pip install -r requirements.txt
```

Run server 

```
python manage.py runserver
```

<h1>Setup Database:</h1>

Install mysql client

```
pip install mysqlclient
```

Change DATABASES IN app/settings.py

```
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'recipe_app_api',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3306'
```

Migrate tables

```
python manage.py migrate
```

<h1>Setup SuperUser:</h1>

```
python manage.py createsuperuser
```
