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


## On production

start containers: 

```
docker-compose -f docker-compose.prod.yml up -d --build
```

stop containers:

```
docker-compose -f docker-compose.prod.yml down -v
```

run migrations:

```
docker-compose -f docker-compose.prod.yml exec web python manage.py migrate --noinput
```
