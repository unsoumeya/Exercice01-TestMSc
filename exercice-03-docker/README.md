# Exercice 03 — Docker WordPress

## Objectif
Déployer un site WordPress à l’aide de Docker Compose en séparant les services
nginx, PHP-FPM et MariaDB afin d’obtenir une architecture propre, modulaire et reproductible.

## Architecture
L’architecture repose sur trois services Docker distincts :
- **MariaDB** : base de données WordPress
- **WordPress (PHP-FPM)** : exécution PHP de l’application
- **Nginx** : serveur web servant les fichiers WordPress et relayant les requêtes PHP

Les services communiquent via le réseau Docker interne.
Les fichiers WordPress sont partagés entre Nginx et PHP-FPM via un volume commun.

## Fichiers fournis
- `docker-compose.yml` : définition de la stack Docker
- `nginx.conf` : configuration du serveur Nginx
- `README.md` : description de l’architecture et du processus

## Déploiement
La stack est lancée à l’aide de la commande suivante :
```bash
docker-compose up -d

