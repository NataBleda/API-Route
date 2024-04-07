Application Symfony avec base de données my_db_symfony

Cette application Symfony est construite autour d'une base de données nommée my_db_symfony qui comprend deux tables principales : Produit et Commande. L'objectif de cette application est de fournir des fonctionnalités CRUD (Create, Read, Update, Delete) pour ces tables, ainsi que des fonctionnalités pour afficher et manipuler les données associées.

Structure de la base de données
La base de données my_db_symfony se compose des tables suivantes :

Produit : Cette table contient des informations sur les produits disponibles, telles que leur nom, leur description, leur prix, etc.

Commande : Cette table représente les commandes passées par les clients. Chaque commande est liée à un client et peut contenir plusieurs produits.

Fonctionnalités
L'application Symfony offre les fonctionnalités suivantes :

Affichage des produits : Vous pouvez visualiser la liste complète des produits disponibles.
Ajout, modification et suppression de produits : Vous pouvez gérer les produits en ajoutant de nouveaux produits, en modifiant les détails des produits existants ou en supprimant des produits de la base de données.
Affichage des commandes : Vous pouvez consulter les commandes passées par les clients, y compris les détails sur les produits inclus dans chaque commande.
Liaison entre Commande et Produit : La relation entre les tables Commande et Produit est de type "One to Many", ce qui signifie qu'une commande peut contenir plusieurs produits.
Routes
Les routes de l'application vous permettent d'accéder aux différentes fonctionnalités CRUD ainsi qu'aux informations sur les commandes et les produits. Voici un aperçu des principales routes :

/produits : Affiche la liste de tous les produits.
/produit/{id} : Affiche les détails d'un produit spécifique.
tu peux utiliser Postman pour manipuler la base de donnés (CRUD);
/commandes : Affiche la liste de toutes les commandes.
/commande/{id} : Affiche les détails d'une commande spécifique.
Installation et Utilisation
Pour utiliser cette application, assurez-vous d'avoir Symfony installé sur votre machine. Voici les étapes à suivre :

Clonez ce dépôt sur votre machine.
Configurez votre base de données dans le fichier .env.
Installez les dépendances en exécutant composer install.
Créez le schéma de base de données en exécutant php bin/console doctrine:schema:create.
Lancez le serveur Symfony en exécutant symfony server:start.
Accédez à l'application dans votre navigateur à l'adresse fournie par Symfony.
Vous êtes maintenant prêt à utiliser l'application Symfony avec la base de données my_db_symfony !
