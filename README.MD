# README

Running:

* Set the environment variables:
VOLUMES
ENVPGDATA
PGPASSWORD
PGUSER

Example:

VOLUMES=/Users/user_name/pg_blog

ENVPGDATA=/Users/user_name/pg_data

PGPASSWORD=12345

PGUSER=postgres

docker-compose -f docker-compose.demo.yml up -d