ready to deploy on heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Set DATABASE_URL variable 

```
DATABASE_URL="sqlite:///posts.db"
DATABASE_URL="postgresql://localhost/flask_example"
```

### Create database

Local

```
>psql
psql> CREATE DATABASE flask_example;
>python db_create.py
```

Heroku

Add postgresql add-on.

```
heroku run bash -a <app_name>
> python db_create.py
```
