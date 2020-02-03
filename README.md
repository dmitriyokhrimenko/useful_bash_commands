# django_learn

### Useful commands 

*deactivate* — Exit out of the current Python virtual envirinment

*workon* — List available virtual envirinments

*workon* **<name_of_environment>** — Activate the specified Python virtual environment

*rmvirtualenv* **<name_of_environment>** — Remove the specified virtual environment.

### Prepare
   
 1/ Install virtual environment.
   
 ```bash
 $ sudo pip3 install virtualenvwrapper
 ```  
   
 2/ Add to /home/{$user}/.bashrc
 
 ```
export WORKON_HOME=$HOME/.virtualenvs 
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3 
export VIRTUALENVWRAPPER_VIRTUALENV_ARGS=' -p /usr/bin/python3 ' 
export PROJECT_HOME=$HOME/Devel 
source /usr/local/bin/virtualenvwrapper.sh
 ```  
   
 3/ Reload .bashrc
 
 ```bash
 $ source ~/.bashrc
 ```
 
 4/ Create venv for project
  
 ```bash
 $ mkvirtualenv <your_venv_name>
 ```
 
 5/ Install Django
  
 ```bash
 $ pip3 install django
 ```
 
 6/ Creating a project directory
  
 ```bash
 $ mkdir <project_dir>
 $ cd <project_dir>
 ```

 7/ Creating a website template
  
 ```bash
 $ django-admin startproject <project_name> .
 $ cd <project_name>
 ```

 7/ Run server
  
 ```bash
 $ python3 manage.py runserver
 ``` 

  Go to the browser at http://localhost:8000

### Your app

 Creating the "catalog" app
  
 ```bash
 $ python3 manage.py startapp catalog
 ``` 
 
 Migrations
  
 ```bash
 $ python3 manage.py makemigrations [<your_app>] - creating the migrations
 $ python3 manage.py migrate - applying migrations
 ``` 
 Creating a superUser
  
 ```bash
 $ python3 manage.py createsuperuser
 ``` 
