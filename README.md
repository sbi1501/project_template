# project_template

## On dev

start containers: 

```
docker-compose up -d --build
```

stop containers:

```
docker-compose down -v
```

run migrations:

```
docker-compose exec web python manage.py migrate --noinput
```
