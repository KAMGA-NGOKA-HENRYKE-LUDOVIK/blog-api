##### **Blog-API**



###### Description



Une API  complète pour la gestion d'un blog, développée avecNode.js, Express et Sequelize. Les données sont stockées dans une base de données SQLite.



Fonctionnalités



\- Lister tous les articles (GET)



\- Rechercher un article par son ID (GET)



\- Créer un nouvel article avec validation des champs (POST)



\- Modifier un article existant (PUT)



\- Supprimer un article (DELETE)



##### Installation et Configuration de l’Environnement Technique



Le développement de l'API a nécessité l'installation de plusieurs outils et bibliothèques via le terminal. Voici les commandes principales exécutées :



###### 1\. Installer les outils 

Aller sur le terminal et entre cette command:



"sudo apt install -y nodejs npm"





Importer tout les dossiers et mettez le dans votre repetoire.

Naviger dans le dossier blog-api sur le terminal et entre la command "npm init -y"



###### 2\. Installer les dépendances 

Installe les paquets nécessaires :



"npm install express sqlite3 swagger-jsdoc swagger-ui-express cors

npm install --save-dev nodemon"



###### 3\. Lancement du serveur:

"npm start"



Vous receverez une réponse qui dit



Connexion à SQLite réussie.

Table articles prête.

Serveur démarré sur http://localhost:3000

Swagger disponible sur http://localhost:3000/api-docs



Sur http://localhost:3000/api-docs, vous pourriez créer, supprimer, modifier les articles.



##### Les Endpoints

Méthode | Endpoint         | Description                             | Paramètres / Corps (JSON)

GET     |/api/articles     |Liste tous les articles                  |Aucun

GET     |/api/articles/:id |Détails d'un article                     |id (dans l'URL)

POST    |/api/articles     |Créer un article                         |"titre, contenu, auteur, date, categorie, tags"

PUT     |/api/articles/:id |Modifier un article                      |id + champs à modifier

DELETE  |/api/articles/:id |Supprimer un article                     |id (dans l'URL)





##### Exemple d'utilisation

Etant sur http://localhost:3000/api-doc

Pour créer un article: cliquez sur "POST" puis sur "try it out". Vous allez vois les different champs et vous les remplissez, après cliquez sur "execute".

Vous recevrez un message de succès.



Pour listé tout les articles: cliquez sur "GET" puis sur "try it out". Vous allez vois des cases, laissez les comme ça et cliquez sur "execute".

Vous allez vois tout les articles.




