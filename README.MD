# README

Functionality: creation of the working environment of the project.

Running:

* Clone app: `git clone git@github.com:mkdevprogects/base.git`
* `cd base/`
* Set the environment variables:
```
  PGUSER  
  PGPASSWORD  
  ENVPOSTGRES_DB  
  VOLUMES  
  ENVPGDATA  
  DB_HOST  
  DB_PG_PORT  
  DB_REDIS_HOST  
  DB_REDIS_PORT  
  HUTCH_MQ_HOST  
  HUTCH_MQ_API_HOST
```  
* `docker-compose -f docker-compose.demo.yml up`
* open browser and go to [http://0.0.0.0:3000/](http://0.0.0.0:3000/) and see patient app
* open browser and go to [http://0.0.0.0:4000/](http://0.0.0.0:4000/) and see manager app
* open browser and go to [http://0.0.0.0:5000/](http://0.0.0.0:5000/) and see history app

Example environment variables:
```
PGUSER=postgres
PGPASSWORD=12345
ENVPOSTGRES_DB=mkdev_dev
```
for running `docker-compose.yml` use 
```
ENVPGDATA=/Users/user_name/pg_data
VOLUMES=/Users/user_name/pg_data
```
and set this environment variables if you run `docker-compose.demo.yml`:
```
DB_HOST=postgres
DB_PG_PORT=5432
DB_REDIS_HOST=redis
DB_REDIS_PORT=6379
HUTCH_MQ_HOST=rabbitmq
HUTCH_MQ_API_HOST=rabbitmq
```