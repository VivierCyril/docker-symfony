# Créer un projet API Symfony avec Docker


# Installation du projet 


## Cloner le dépôt du projet

```bash
git clone <lien>
```
## Créer une image docker

```bash
docker compose build
```
## Créer un container avec les services 

```bash
docker compose up -d
```
## Connectez vous au conteneur 

```bash
docker exec -it php8-symfony bash
```
## Installer les dépendances Symfony

```bash
composer install
```

## Vérification du container et des services

Rendez-vous sur les liens 

- http://localhost:8080 : Lien vers symfony
- http://localhost:9000 : Lien vers phpMyAdmin