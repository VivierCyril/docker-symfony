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
  DATABASE_URL=
```
