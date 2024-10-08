

# Gestion Recette API

Cette API permet de gérer des recettes avec des opérations de création, de lecture, de mise à jour et de suppression (CRUD).

## Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- [Node.js](https://nodejs.org/) (version 14 ou supérieure)
- [MySQL](https://dev.mysql.com/downloads/installer/) (version 5.7 ou supérieure)
- Un outil de gestion de requêtes API comme [Postman](https://www.postman.com/) ou `curl`.

## Endpoints de l'API

**Récupérer toutes les recettes**

- Méthode : GET
- Endpoint : /api/recettes
- Description : Récupère la liste de toutes les recettes.

Exemple de requête :

```
GET http://localhost:3000/api/recettes
```

**Récupérer une recette par ID**

- Méthode : GET
- Endpoint : /api/recettes/:id
- Description : Récupère les détails d'une recette spécifique en fonction de son ID.

Exemple de requête :

```
GET http://localhost:3000/api/recettes/1
```

**Créer une nouvelle recette**

- Méthode : POST
- Endpoint : /api/recettes
- Description : Crée une nouvelle recette avec les données fournies dans le corps de la requête.

Exemple de requête :

```
POST http://localhost:3000/api/recettes

{
  "titre": "Pancakes",
  "ingredients": "Farine, lait, œufs",
  "type": "plat"
}
```
**Mettre à jour une recette par ID**

- Méthode : PUT
- Endpoint : /api/recettes/:id
- Description : Met à jour une recette spécifique en fonction de son ID

Exemple de requête :

```
PUT http://localhost:3000/api/recettes/1


 {
        "titre": "nouvelle recette5",
        "ingredient": "Pâte brisée, Lardons",
        "type": "plat"
 }
```
**Supprimer une recette par ID**

- Méthode : PUT
- Endpoint : /api/recettes/:id
- Description : Supprime une recette spécifique en fonction de son ID.

Exemple de requête :

```
DELETE http://localhost:3000/api/recettes/1
```

**Récupérer toutes les categories**

- Méthode : GET
- Endpoint : /api/categories
- Description : Récupère la liste de toutes les categories.

Exemple de requête :

```
GET http://localhost:3000/api/categories
``

**Créer une nouvelle categorie**

- Méthode : POST
- Endpoint : /api/categories
- Description : Crée une nouvelle categorie avec les données fournies dans le corps de la requête.

Exemple de requête :

```
POST http://localhost:3000/api/categories

{
  "nom": "Dessert"
}
```

## Installation

- Clonez le dépôt sur votre machine locale :

```
https://github.com/OusmaneLyDev/gestion-recette-api.git
```

```
cd gestion-recette-api
```

- Installer les dépendances

```
npm install
```

- Configurer l'environnement
  Créez un fichier .env à la racine du projet et ajoutez les configurations nécessaires (par exemple, pour la base de données).

- Exemple .env :

```
DB_HOST=localhost
DB_DATABASE=database_name
DB_USERNAME=username
DB_PASSWORD=password
```

- Démarrer le projet

```
npm start
```

L'API sera accessible à [http://localhost:3000](http://localhost:3000)

- Exécution des tests unitaires

Exécuter les tests

Lancez les tests avec la commande suivante :

```
npm test
```

L'application sera disponible à http://localhost:3000.

## Auteur

[Ethman Ly](https://github.com/OusmaneLyDev).
