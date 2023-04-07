# DRF Cinema API
API service for managing cinema written on DRF

## Installing using GitHub
Install PostgresSQL and create database

```
git clone https://github.com/derkach55/cinema-api.git
cd cinema-api
python -m venv venv
source venv/bin/activate (on Linux)
venv\Scripts\activate (on Windows)
pip install -r requirements.txt
set POSTGRES_DB=<your db name>
set POSTGRES_USER=<your db user>
set POSTGRES_PASSWORD=<your db password>
set POSTGRES_HOST=<your db host>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver 
```

## Run with Docker
Docker must be installed

```
docker-compose up --build
```

## Getting access

* create user via /api/user/register/
* get access token via /api/user/token/

## Features

* JWT authentication
* Admin panel
* Documentation at api/doc/swagger/
* Managing orders and tickets
* Creating movies, cinema halls, actors and genres
* Adding movie sessions
* Filtering movies and movie sessions
