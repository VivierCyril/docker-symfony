# Initialisation

Run the docker-compose

```bash
docker-compose build
docker-compose up -d
```


Log into the PHP container

```bash
docker exec -it php8-sf6 bash
```

Install dependency

```bash
composer install
```

If you need a database, modify the .env file like this example:

```yaml
  DATABASE_URL="postgresql://symfony:ChangeMe@database:5432/app?serverVersion=13&charset=utf8"
```

Configue ENV.LOCAL

```python
###> Docker/environnement ###
###> MYSQL
MYSQL_ROOT_PASSWORD=secret
MYSQL_DATABASE=api
MYSQL_USER=apiroot
MYSQL_PASSWORD=secret

###> PHPMYADMIN
PMA_ARBITRARY=1
PMA_HOST=db
PMA_USER=apiroot
PMA_PASSWORD=secret
MYSQL_ROOT_PASSWORD=secret

###> doctrine/doctrine-bundle ###
DATABASE_URL="mysql://apiroot:secret@db:3306/api?serverVersion=8.0"
```