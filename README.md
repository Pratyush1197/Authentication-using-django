# Authentication-using-django
This is a project which will provide authentication to users through a token generated. All the requests are fired through Postman


$ git clone https://github.com/Pratyush1197/Authentication-using-django.git

$ cd Authentication-using-django/

$ virtualenv --python=`which python3` venv

$ source venv/bin/activate

$ pip install -r requirements.txt

$ cd myproject

$ python manage.py migrate

$ python manage.py runserver
```
Application is started at 
``
127.0.0.1:8000
After this open Postman and send a POST request with the username and password specified in body, to 127.0.0.1:8000/auth/login. 
A token will be generated
Use this token to send GET request to 127.0.0.1:8000/auth/test
If the credentials are correct you will get the Welcome message
