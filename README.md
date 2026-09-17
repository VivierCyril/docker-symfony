# Initialisation

Cloner le dépôt 

```bash
git clone <lien>
```

Créer une image docker

```bash
docker-compose build
```
Créer un container avec les services 

```bash
docker-compose up -d
```

Connectez vous au conteneur 

```bash
docker exec -it php8-symfony bash
```

Installer les dépendances Symfony

```bash
composer install
```
Ajouter la variable DATABASE_URL du fichier .env en adéquention avec le docker-compose.

