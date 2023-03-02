# Cinema API
API service for cinema management written on DRF

## Features
- JWT authentication
- Admin panel /admin/
- Documentation /api/doc/swagger/
- Creating movies with genres and actors
- Creating movie halls
- Adding movie sessions
- Managing tickets and orders
- Filtering movies and movie sessions

## Install using GitHub
Install PostgreSQL and create database
Use `.env.sample` as example and create file `.env` with your settings
```
git clone https://github.com/ansicat/cinema-api.git
cd cinema-api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
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
