# INF3080 edition Automne 2019
INF3080 Bases de données

## Objectifs
Introduire les concepts fondamentaux des bases de données relationnelles.

## Sommaire du contenu
Information, données et système de gestion de bases de données (SGBD). Présentation des principales architectures de bases de données.

Modèle entité-association. Modèle relationnel. Algèbre relationnelle et langage SQL. Contraintes d'intégrité et gâchette (trigger). Création, exploitation et administration d'une base de données. Schéma interne : indexage et hachage. Intégration d'une base de données dans une application. Sécurité. Transactions. Évaluation et optimisation des requêtes relationnelles.

### Plan de cours
+  1 : Introduction aux systèmes de gestion de bases de données (nom, type, rôle et environnement)
   - Neo4J, SQLite, SQL Server, Oracle, PostgreSQL, Kyoto Cabinet
+  2 : Introduction au modèle entité-association
+  3 : Introduction au modèle relationnel
   - schéma, formes normales, normalisation vs dénormalisation, notation, type de données
   - se familiariser avec les 12 règles de Codd
+  4 : Introduction à l'algèbre relationnelle
+  5 : Introduction à Oracle et SQL*plus dans un environnement Linux
   - connexion, commandes de base, scripts
   - Les objets système du SGBDR Oracle
   - La requête la plus simple : SELECT * FROM DUAL;
+  6 : Le langage SQL partie DDL (CREATE, DROP, ALTER) 
   - table, view, index, sequence, contrainte, intégrité
+  7 : Le langage SQL
   - partie DML (INSERT, DELETE, UPDATE)
   - partie TCL (COMMIT, ROLLBACK, ...)
   
+ Mi-Session

+  8 : Le langage SQL et les requêtes avancées
   - filtre, jonction, groupement, sous-requête
   - Initiation au PL/SQL et les fonctions
+ 9 : La programmation PL/SQL pour la création de gâchettes
+ 10 : La programmation PL/SQL pour la création de procédures et packages
+ 11 : La programmation PL/SQL Les curseurs
+ 12 : Droits et sécurité des objets
  - partie DCL (GRANT, REVOKE)
+ 13 : Introduction à SQL*Net et les connecteurs
   - Connectivité à partir d'une application distante
   - Les applications 2-tiers vs 3-tiers
+ 14 : Coût et optimisation de requêtes
  - Explain plan
  - Les indexes vs table scan
+ 15 : Introduction et théorie des entrepôts de données
  - Schéma en étoile, table maître et table de faits, modélisation

+ Fin de session.

### Modalités d'évaluation proposées 

#### Examens
 + Examen Intra (#1) : 30%, 26 octobre 2019 de 14:00 à 17:00
 + Examen Final (#2) : 30%, 14 décembre 2019 de 14:00 à 17:00

##### Directives aux examens
 + Avoir votre carte d'étudiant UQAM valide;
 + Une feuille (format lettre) recto verso de notes personnelles est permise; (pourrait changer)
 + Vous ne pouvez pas collaborer avec un partenaire;
 + Vous ne pouvez pas prendre les notes personnelles d'un voisin;
 + Bien lire les questions;
 + Vous devez réfléchir avant de répondre;
 + Répondre dans les espaces prévus;
 + Vous avez trois (3) heures;
 + **Signez la feuille de présence avant votre départ.**
 
#### Travaux :
 + Travail pratique #1 : modélisation 25%
 + Travail pratique #2 : réalisation 15%
 
##### Directives des travaux :
 + Remise électronique (privé) via GitHub.com

### Références
 - https://info.uqam.ca/politiques/
 - https://www.researchgate.net/scientific-contributions/70214812_E_F_Codd
 - https://computing.derby.ac.uk/c/codds-twelve-rules/
 - Oracle technet
 - Robert Godin, UQAM, Professeur
