# Docker repository for taco team

### Intallation

***Installez*** la Community Edition de [Docker, ici](https://www.docker.com/community-edition)

***

Ensuite, téléchargez le repo de l'application meteor dans le dossier `data` avec la commande ci-dessous :

```bash
git clone https://github.com/AmFlint/taco-application.git ./data/application
```

Une fois le projet installé, vous devrez installer les dépendances dans le dossier

```bash
npm install
```

### Accéder aux services de l'application

Maintenant, revenez à la racine du repo docker et lancez la commande :
```bash 
docker-compose up
```

Les serveurs front, back vont se lancer en même temps que la base de donnée mysql et phpmyadmin.

Pour accéder aux services:
  - Application [http://localhost:3000](http://localhost:3000)
  - Interface Administration MongoDB [http://localhost:8080](http://localhost:8080)
  - MongoDB disponible sur le port 27017

Credentials for MongoDB Database:
  - database name: taco
  - username: admin
  - password: pass

***Notez*** que vous devrez ouvrir les dossier présents dans `./data` dans vos éditeurs de texte, après chaque modifications, les serveurs seront redémarrés pour prendre en charge les modifications.

### Eteindre les services :

```bash
docker-compose down
```

***Notez*** que les données stockées dans la base de donnée seront persistées et seront sauvegardées en local après l'extinction des services.

