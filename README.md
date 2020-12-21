# pp sabov cs-215
## Instructions
1. Create and activate a virtual environment on your machine:
```shell script
virtualenv <name-of-env> -p <path/to/python/binary>
source venv/bin/activate
```
By typing `which python` you can ensure that using the virtual environment.

2. Install the needed packages:
```shell script
python -m pip install -r requirements.txt
```

3. Run:
```shell script
export FLASK_APP=application/application.py
flask run
```
For a production environment, you should use a WSGI server, for example
Gunicorn (which is installed as a dependency):
```shell script
cd application
gunicorn application/application:app
```

__To run application after laba 7__
* ######Windows
```
venv\Scripts\activate
alembic lalala...
cd application
set FLASK_APP=application.py  
set FLASK_DEBUG=1
flask run
```

* ######Linux
```
venv\bin\activate
alembic lalala...
cd application
export FLASK_APP=application.py  
export FLASK_DEBUG=1
flask run
```

Use file  _lab7templates.txt_  to make your life easier