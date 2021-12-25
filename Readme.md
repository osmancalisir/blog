django commands:
py manage.py makemigrations --dry-run --verbosity 3
py manage.py runserver
py manage.py createsuperuser
pip install coverage
coverage run --omit='*/venv/' manage.py test
coverage html
pip install djangorestframework
------------------------------------
React commands
npx create-react-app blogapi .
cd blogapi
npm start
npm install react-router-dom
npm install @material-ui/core
pip install django-cors-headers


------------------------------------
py -m venv venv
venv\Scripts\activate
pip install django
django-admin startproject core .
django-admin startapp blog
django-admin startapp blog_api
py manage.py runserver
py manage.py makemigrations
py manage.py migrate
py manage.py createsuperuser