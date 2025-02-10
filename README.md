# dockerdjango

Testing some stuff

## Create new webapp Directory
```
cd …
mkdir webappname
cd webappname
code .
```

## Environment

Setup virtual environment
```
python -m venv envname
/envname/Scripts/activate
```
Then install django
```
(envname) python -m pip install Django
```

## Django

```
# Start a project
django-admin startproject projectname .
```
```
# Build an application within project
python manage.py startapp appname
```
```
# Migrations
python manage.py managemigrations
python manage.py migrate

```
```
# Spin up Server
python manage.py runserver
```

## Docker

### buildx

Some basic buildx commands are:
```
docker buildx ls
```
```
docker buildx create --name testbuilder
```
```
docker buildx use testbuilder
```
```
docker buildx build --platform linux/amd64,linux/arm64,linux/arm/v7 -t username/imagename --push .
```