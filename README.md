### README pour le Dépôt de l'Application Node.js

---

# Application de Prise de Notes

Cette application est une simple application web de prise de notes construite avec Node.js et Express. Elle est conçue pour démontrer la mise en place d'un pipeline CI/CD avec GitHub Actions.

## Prérequis

- Node.js (version 14 ou supérieure)
- Docker
- Un compte GitHub
- Un compte Docker Hub
- Un compte Heroku (facultatif)

## Installation

1. Clonez le dépôt GitHub :

```sh
git clone <URL_DU_DÉPÔT>
cd <NOM_DU_DOSSIER>
```

2. Installez les dépendances Node.js :

```sh
npm install
```

## Exécution de l'Application

Pour démarrer l'application en local, exécutez :

```sh
npm start
```

L'application sera accessible sur http://localhost:3000.

## Tests

Pour exécuter les tests unitaires, utilisez :

```sh
npm test
```

## Docker

### Construction de l'Image Docker

Pour construire l'image Docker de l'application, exécutez :

```sh
docker build -t sample-app .
```

### Exécution de l'Application avec Docker

Pour exécuter l'application dans un conteneur Docker, utilisez :

```sh
docker run -p 3000:3000 sample-app
```

L'application sera accessible sur http://localhost:3000.

### Push de l'Image Docker vers Docker Hub

1. Connectez-vous à Docker Hub :

```sh
docker login -u <votre_nom_d'utilisateur>
```

2. Poussez l'image Docker :

```sh
docker tag sample-app <votre_nom_d'utilisateur>/sample-app:latest
docker push <votre_nom_d'utilisateur>/sample-app:latest
```
