

 Application de Gestion de l'État Civil

Cette application permet de gérer l'état civil des citoyens d'une province, y compris les informations sur les hommes, les femmes, et les mariages.

Fonctionnalités
- Gestion des entités `Homme`, `Femme`, et `Mariage`.
- Affichage des épouses d'un homme entre deux dates.
- Nombre d'enfants d'une femme entre deux dates.
- Identification des femmes mariées deux fois ou plus.
- Nombre d'hommes mariés à quatre femmes entre deux dates.
- Détails des mariages d'un homme, y compris mariages en cours et échoués.

 Structure du Projet
- Couche de Persistance :
  - Entités dans `ma.projet.beans` avec les annotations appropriées.
  - Configuration Hibernate dans `hibernate.cfg.xml`.
  - Classe `HibernateUtil` dans `ma.projet.util` pour la gestion de la session.
- Couche Service :
  - Interface `IDao` dans `ma.projet.dao`.
  - Services : `HommeService`, `FemmeService`, `MariageService` implémentant `IDao`.

 Installation
1. Créer la base de données sous MySQL.
2. Développer les classes d'entités avec les annotations vues en classe.
3. Configurer le fichier `hibernate.cfg.xml` pour la connexion à la base de données.
4. Mettre en place les classes de service et les méthodes décrites.

 Test
- Créer 10 femmes et 5 hommes.
- Exécuter les tests pour afficher les listes et les informations demandées.
