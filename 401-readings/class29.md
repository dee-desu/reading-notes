# read 29: API Deployment
## API Deployment

### This article is intended for engineers who use the Django framework. It gives a deep insight into configuring Django project settings, and the pros and cons of different approaches.

### In the article, you will also find recommendations concerning tools, best practices, and architectural solutions, all time-tested and proven by successful projects. And if you still have questions after reading it, you can always leave a comment below or use our contact form. The article is based on Django Stars’ vast experience with real projects. Our dedicated teams are ready to speed up your development project.



## Managing Django Settings: Issues
### Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.



### Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

### Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.




### Django settings are a Python code. This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.

### Setting Django Configurations: Different Approaches
### There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best. Let’s take a brief look at the most popular ones to examine their weaknesses and strengths.

### settings_local.py
### This is the oldest method. I used it when I was configuring a Django project on a production server for the first time. I saw a lot of people use it back in the day, and I still see it now.

### The basic idea of this method is to extend all environment-specific settings in the settings_local.py file, which is ignored by VCS. Here’s an example:

### settings.py file:


```python
ALLOWED_HOSTS = ['example.com']
DEBUG = False
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'production_db',
        'USER': 'user',
        'PASSWORD': 'password',
        'HOST': 'db.example.com',
        'PORT': '5432',
        'OPTIONS': {
            'sslmode': 'require'
        }
    }
}
...
from .settings_local import *
```

### settings_local.py file:



```python
ALLOWED_HOSTS = ['localhost']
DEBUG = True
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'local_db',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```
### Pros:
### Secrets not in VCS.
### Cons:
### settings_local.py is not in VCS, so you can lose some of your Django environment settings.
### The Django settings file is a Python code, so settings_local.py can have some non-obvious logic.
### You need to have settings_local.example (in VCS) to share the default Django configurations for developers.
### Separate settings file for each environment
### This is an extension of the previous approach. It allows you to keep all configurations in VCS and to share default settings between developers.

### In this case, there are multiple files from which projects on Django get settings, and you make a settings package with the following file structure:

```
settings/
   ├── __init__.py
   ├── base.py
   ├── ci.py
   ├── local.py
   ├── staging.py
   ├── production.py
   └── qa.py
```
### settings/local.py:
```python
from .base import *
ALLOWED_HOSTS = ['localhost']
DEBUG = True
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'local_db',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```
