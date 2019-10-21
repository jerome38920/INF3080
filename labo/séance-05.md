##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 5: Langage SQL - DML

- Objectif : Expérimenter le DDL et la création de script
   
----
**Note** : (_facultatif_) S'il y a des questions dans ce labo, répondez y dans un fichier nommé
`./labo/reponse-labo.md`.  Le fichier doit être dans un format `Markdown`. Utilisez le projet
`in3080-a2019` pour déposer le fichier demandé. Utiliser le même fichier pour tous les exercices.

##### Format du fichier Markdown
 + Séance 2 (Header 1)
 + Exercice {1..n} (H2)
 + Question {1..n} (H4)
 + S`2`.E`3`.Q`1` (strong) `est une valeur qui change bien sûr`
 + La réponse dans une section script (code block)

**Note**: Il est recommandé de versionner vos réponses aux exercices à l'aide
de Git. Un seul dépôt est amplement suffisant pour tous les laboratoires, en
divisant les fichiers dans des répertoires.

 > > Pourquoi versionner vos exercices avec Git: afin de
vous entraîner à utiliser le logiciel (commandes) naturellement.

----

## 0 - Directives

+ Faites le maximum selon vos connaissances;
+ Lire l'atelier completement;
+ Débuter le devoir;

## 1 - Création du script (à partir du modèle gestion des accès)

Vous devez créer le schéma à partir du modèle relationnel (modèle entité association) [modèle A](./modele_labo.png).  Votre script
sera nommé `01_schema.sql`.  Ce script vous permettera de créer les objets nécéssaire pour opérationnalisé une BD performante.

![modèle A](./modele_labo.png)

+ a) Créer les tables avec les attributs;
+ b) Créer les clés primaires dans le CREATE TABLE pour 3 entités;
+ c) Créer les clés primaires avec ALTER TABLE pour 3 entités;
+ d) Ajouter les contraintes;
+ e) En terminant, créer les indexes pour chacunes des tables;

#### Questions :

- Q1. Temps pour réaliser ce devoir ?
- Q2. Difficultés rencontrées ?

### FIN.

---

Auteur Guy Francoeur :copyright: version A2019
