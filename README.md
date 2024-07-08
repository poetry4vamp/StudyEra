### Create a folder on your desktop, named it 'django'

### Go to the folder and type cmd on the folder path

### Type in the terminal,
        py -m venv venv
        venv\scripts\activate
        pip install django
        
### Update django version if needed, then type in the terminal
        django-admin startproject studentstudyportal
        cd studentstudyportal
        django-admin startapp dashboard
        
### Open the project
### Install python extension in vscode, then type in  the terminal
        py manage.py createsuperuser (create your own admin credentials to access)
        pip install crispy-bootstrap4
        pip install requests
        
### Modify the INSTALLED_APPS of settings.py (see the 'settings.py' file in the folder)
### Add these at the bottom part of settings.py 

        STATIC_URL = '/static/'

        STATICFILES_DIRS=[BASE_DIR/"static"]
        
        LOGIN_REDIRECT_URL = 'home'
        
        LOGIN_URL = 'login'

        CRISPY_TEMPLATE_PACK = "bootstrap4"
    
### Modify imports and urlpatterns of urls.py (see the 'urls.py' file in the folder), and type in the terminal
        py manage.py makemigrations
        py manage.py migrate
        
### If both makemigrations and migrate don't work, try to copy the files in migrations folder to your migrations folder, then type
        py manage.py runserver 
    
    
    
