# Cinema API
API service for cinema management written on DRF

## Features
- JWT authentification
- Admin panel /admin/
- Documentation /api/doc/swagger/
- Creating movies with genres and actors
- Creating movie halls
- Adding movie sessions
- Managing tickets and orders
- Filtering movies and movie sessions

## Install using GitHub
Install PostgreSQL and create database
```
git clone https://github.com/ansicat/cinema-api.git
cd cinema-api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set POSTGRES_HOST=<db host>
set POSTGRES_DB=<db name>i
set POSTGRES_USER=<db user>
set POSTGRES_PASSWORD=<db user password>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run with Docker
Use `.env.sample` as example and create file `.env` with your settings
```
docker-compose build
docker-compose up
```

## Getting access
- create user /api/user/register/
- get access token /api/user/token/
- list of endpoints /api/cinema/
