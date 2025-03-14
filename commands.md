find . -path "*/migrations/*.py" -not -name "__init__.py" -delete
find . -path "*/migrations/*.pyc"  -delete
python manage.py dbshell
sqlite> .table
sqlite> DROP TABLE <table>;



![alt text](image.png)


[
    1. Sign up || http://127.0.0.1:8000/auth/users/
    2. Login || http://127.0.0.1:8000/auth/token/login/
    3. Profile || http://127.0.0.1:8000/auth/users/me/
    4. Set password || http://127.0.0.1:8000/auth/users/set_password/
    5. Set username || http://127.0.0.1:8000/auth/users/set_username/
]

#Creating Categories


python manage.py makemigrations [app]
python manage.py migrate [app]
pip freeze > requirements.txt
pip install -r requirements.txt