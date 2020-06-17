# Create Django Project 
docker-compose run web django-admin startproject myDocker .

# Create Django App

docker exec titan_web_1 python manage.py startapp pages

# Migration
docker exec titan_web_1 python manage.py makemigrations
docker exec titan_web_1 python manage.py Migrate

# RunProject(Docker Compose)
docker-compose up
docker-compose down

# ----------------PostGrace-----------------------
docker exec -it titan_db_1 bash
psql -U postgres
# Check database
\l
# connect database
\c databasename

# show tables
\dt




